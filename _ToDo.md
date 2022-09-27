## Manage Bibtex import https://wowchemy.com/docs/managing-content/#create-a-publication

Install academic


pip3 install -U academic
pip3 show academic

bibtool -s -d ~/Documents/Biblio/Zotero/library.bib -o library-html.bib 
bib2bib -oc sdray-arti -ob Publications.bib -c 'author : "Dray"' library-html.bib
rm library-html.bib
rm sdray-arti

export PATH="/home/$USER/.local/bin/:$PATH"
academic import --bibtex Publications.bib

## Todo 
* add publication / adress for talks/seminar (they have been removed by academic import)

## Syncing publications (from https://jc-castillo.com/post/zotero-academic/)

## 1. Getting and sync your publications from a reference manager

(if you already have a bib file and you do not intend to automatize this process, proceed to step 2)

One of the things that academics hate is to deliver information from publications in different formats all the time (university forms, project reports, CVs, etc), very annoying and time consuming. If populating a website means to write a different record for any publication AGAIN ... no way. Therefore, I believe the best way to do this is to keep your own references saved just once in a reference manager and then link the information from there. I recommend [Zotero](https://www.zotero.org/) for its excellent quality, for being open source, and because it allows to keep collections/subcollections files synced in any place in your computer thanks to the plug-in Better BibTex.

I won't cover here the use of Zotero or BetterBibTex (BBT) in detail, there are excellent tutorials for this. I will just focus on some recommendations and options of BBT in order to automatize the incorporation of publication records on your academic website. The final goal is that:

- you add a bibliographic reference to Zotero
- you run a simple script (see below)
- you get your publications rendered in your academic website

### Save your academic references in a folder/subfolder

Zotero allows to organize your references in folders, which then can be exported independently to other formats. I recommend to create a folder called `academic-publications` where you can save or move bibliographic records where you are one of the authors. You can choose another name for the folder but I recommend this because to keep coherence with the following workflow. This is the folder that contains the information that will be published in your website.

### Export a synced `bibtex` file from your Zotero folder.

The academic-website requires a bibtex file as an input for generating publication records. In order to keep this file synced with your Zotero collection you can use the Zotero add-in [BetterBibTex](https://retorque.re/zotero-better-bibtex/). Once installed, a bit of customization in Tools > Preferences > BetterBibTex tab

- in Export tab
  - Bibtex tab uncheck "Export unicode ...", otherwhise there are problems with special characters
  - Add URLs to Bibtex export: select in the URL field

- in Miscellaneous tab (within Export, not the other one)
  - uncheck "Apply case-protection to capitalized words by enclosing them in braces"

Now we are ready to export the collection:

  - right click over your Zotero folder _academic-publications_
  - format: Better BibTex
  - select "Keep updated"
  - ok, and save it under your project folder content/publication

These steps create an `academic-publications.bib` file in your website folder. Any reference that you add afterwards, as well as any modification to any of your record, it will updated with the bibtex file available for your website.

Finally, this assumes that you have a relatively ordered and completed set of references. Please check, in my case sometimes authors' names appear written differently in different references, which for a bibtex file means two different authors. I also recommend to add an abstract to each reference, as it is the body of the publication record in your website. There is no need to do this at the beginning as further updates on Zotero will be reflected in your website after the following step.

So far I have tried this with the followig entries: journal, books, chapters and reports, and they are rendered pretty well.

## 2. `bibtex_2academic` R script

This R script consists of an R function based on the one by [Busetto](https://www.r-bloggers.com/2018/03/automatically-importing-publications-from-bibtex-to-a-hugo-academic-blog-2/) which basically extracts information from each Bibtex record stored in a .bib file and generates a markdown file incorporated as publication in the academic theme.

The first part of the script creates the function `bibtex_2academic` and the second runs the script specifying a) the bib file, and b) the folder where the publication records (as markdown files) are saved. The script uses the `pacman` package to install/load libraries, so if it is not installed the script does it and it might take a while just the first time.

The default way to do this is:

- save the [bibtex_2academic.R](https://raw.githubusercontent.com/juancarloscastillo/starter-hugo-academic/master/content/publication/bibtex_2academic.R) file in the content/publication folder (part of the default folders)
- save your bib file in the same folder with the name `academic-publications.bib` (details in previous step)
- run the script from R. Assuming that your working directory is the root folder of the website project, run: `source("content/publication/bibtex_2academic.R")`

After running the script, the publication folder should have as many markdown files as the number of references in your Zotero synced folder (and in your generated bib file). After rendering the site with blogdown (`blogdown::serve_site()` from terminal) you should be able to see the list of publications rendered in the default widget "Recent publications" and in `[your website address]/publications/`

## About the overwriting option

There are two approaches for this citations-academic workflow: 1) to generate the markdown files and then to add additional details and customization there to each markdown file, or 2) make all the modifications within Zotero and do not touch the markdown files generated by this script. Although the first approach allows to add some more fancy stuff manually, I prefer to use the second one and only add information and modifications within Zotero. But, if you go for the first one you should change the "overwrite" option at the end of the script to _false_, otherwise any change you make locally in the bib file will be lost when running the script again.

## Update: add conferences and presentations

I wasn't sure whether to make a different tab for each type of academic production (papers, presentations, conferences), but at the end I decided to make just one big archive of "academic production" as they can be easily sorted within the same page with the drop-down button. It was more complicated than I thought, as some Zotero types where not well recognized by the script and by Wowchemy. So, this is what I did:

- Conference presentations are registered in Zotero as "conference papers", other talks as "presentations"
- Conferences papers works fine, but presentations are a Zotero type which is not recognized in bibtex records. I changed the script and passed the "Misc" (miscellaneous category) to "Presentations". Still, this is not recognized by Wowchemy so I followed the instructions to [change options in the language pack](https://wowchemy.com/docs/hugo-tutorials/language/):
  - create a i18n folder in the root
  - save here the english language file **en.yaml** from [here](https://github.com/wowchemy/wowchemy-hugo-themes/blob/main/wowchemy/i18n/en.yaml)
  - in `id: pub_uncat` change translation from "Uncategorized" to "Presentation"
  - the details of the presentation (as place, etc) should be added to the "type" field in Zotero
  
  