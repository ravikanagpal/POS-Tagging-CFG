

#  A list of all the resources used


-   https://stackoverflow.com/questions/33207799/nltk-cant-interpret-grammar-category-prp-output-by-stanford-parser - To include dollar as non terminal

-   https://www.nltk.org - For looking at NLTK APIs

-   https://web.stanford.edu/~jurafsky/slp3/12.pdf - To look at constituency grammar

-   https://developers.google.com/machine-learning/crash-course/classification/precision-and-recall - For understanding precision and recall tug-of-war

-   https://www.nltk.org/book/ch08.html - To understand grammar parsing (nltk chart parsing)

-   https://www.kite.com/python/answers/how-to-read-a-tsv-file-in-python - To find out how to read TSV file. 


#  Execution Instructions

## Setup
```sh
# Setup python virtual environment
$ virtualenv venv --python=python3
$ source venv/bin/activate

# change directory to the repo where we have requirements file
$ cd POS-Tagging-CFG/

# Install python dependencies
$ pip3 install  -r requirements.txt 

```

## Run
Use the following command in the current directory.

`python3 src/main.py data/train.tsv grammars/toy.cfg output/train.tsv`

## Data

The assignment's train data can be found in [data/train.tsv](data/train.tsv).

## Output

The output is stored in tsv file and can be found in [output/train.tsv](output/train.tsv)


