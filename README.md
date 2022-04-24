# data-mining-project

First, I downloaded the abstracts as .txt file from PUBMED (for github, Had to compress the txt file from pubmed as it was >25mb.). then I extracted the pmid for each abstract and stored them in pmid files. The pmid extraction code is in cell 1 of the jupyter file (try1.ipynb) in the folder try1-basic codes.

Annotate_using_PubTator.py is the code for annotating based on pmid. It takes pmid files as input. each pmid file has 100 pmids only because the API accepts 100 per request. It gives annotatedabstracts.txt as output.


Once the pmid files are generated (pmids.zip on github), run SubmitPMIDList.py to get the annotated text.


gene.csv: names of all the genes
protein.csv: names of all the proteins
woundabstracts.csv: all 10k abstracts
annotatedabstracts.txt: annotated the 10K abstracts


The next cells in the jupyter file:

wait for a minute for the jupyter output to load on github

I Converted the 10000 abstracts from txt to csv file "woundabstracts.csv". So the first cell in jupyter can be commented. (don't comment the libraries)

must execute "conda install -c conda-forge spacy-model-en_core_web_sm" to install spacy package.

Tried using gensim and checked similary of "wound" with different proteins,genes.

## Then I checked the similarity between those proteins and genes.

try1 is the jupyter file. The red marked text in the output are not errors but just time log. 


I tried with just 10k abstracts for now. And the parameters must be tuned.

todo: try with bigrams also. use phrases library for that
