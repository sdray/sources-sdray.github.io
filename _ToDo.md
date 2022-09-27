## Manage Bibtex import https://wowchemy.com/docs/managing-content/#create-a-publication

Install academic


pip3 install -U academic
pip3 show academic

## update my publications with zotero and put in the list academic-publications folder (with automatic update to the bib file)

export PATH="/home/$USER/.local/bin/:$PATH"
academic import --bibtex academic-publications.bib

## Todo 
* add publication / adress for talks/seminar (they have been removed by academic import)
