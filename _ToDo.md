## Manage Bibtex import https://wowchemy.com/docs/managing-content/#create-a-publication

pip3 install -U academic
pip3 show academic

export PATH="/home/$USER/.local/bin/:$PATH"
academic import --bibtex Publications.bib

## Todo 
* add publication / adress for talks/seminar (they have been removed by academic import)