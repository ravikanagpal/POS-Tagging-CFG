# Intro to NLP - Assignment 2

## Team
|Student name      | CCID       |
|------------------|------------|
|Ravika Nagpal     |  ravika    |
|Seeratpal Jaura   |  seeratpa  |

# 2. A list of all the resources used


-   https://stackoverflow.com/questions/33207799/nltk-cant-interpret-grammar-category-prp-output-by-stanford-parser - To include dollar as non terminal

-   https://www.nltk.org - For looking at NLTK APIs

-   https://web.stanford.edu/~jurafsky/slp3/12.pdf - To look at constituency grammar

-   https://developers.google.com/machine-learning/crash-course/classification/precision-and-recall - For understanding precision and recall tug-of-war

-   https://www.nltk.org/book/ch08.html - To understand grammar parsing (nltk chart parsing)

-   https://www.kite.com/python/answers/how-to-read-a-tsv-file-in-python - To find out how to read TSV file. 


# 3. Execution Instructions

## Setup
```sh
# Setup python virtual environment
$ virtualenv venv --python=python3
$ source venv/bin/activate

# change directory to the repo where we have requirements file
$ cd f2021-asn2-ravikanagpal/

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

# 4. Design Discussions

-   We discussed the assignment and divided the data sentences to build cfg grammar.
-   We identified issue with adding dollar sign to non-terminal and double quotes to the terminal symbol, for which we looked at stackoverflow resources (as specified under list of resources).
-   We then identified the rules to be added to CFG grammar (toy.cfg file) based on the senetences in the data
-   We looked at the false positive, false negatives , true positives and true negative number for each rule to check their effect on precision and recall.
-   To reduce the overfitting issues, we analyzed False positive and False negative after adding each rule to the grammar. 
-   We used google colab notebook to do the practice work of running those grammar rules and the combination of those rules to identify good rules.
-   To write down our error analysis report, we noted down the examples, behaviours and reasons for getting false positives and false negatives while analysing our grammar rules.

# 5. Report 

The report is a pdf, named as "Evaluation and Error Analysis Report" (found in the same directory as ReadMe)[report](https://github.com/UOFA-INTRO-NLP-F21/f2021-asn2-ravikanagpal/blob/main/Evaluation%20and%20Error%20Analysis%20Report.pdf).
