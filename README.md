# Setup
This repository is a dump of many of the code snippets used in the Big Data NLP talk at KDD in 2016. Feel free to reach out to us with questions, improvements, or suggestions.

Here's a list of modules we'll be using in ipython notebooks. This will function with any Operating System.

Install Python 2.7 and some module dependencies 
    pip install ipython nltk networkx zss datasketch agglomcluster
    # This is slow, the wordnet dependency is large consider downloading after talk
    python -e "import nltk; nltk.download('punkt'); nltk.download('wordnet'); nltk.download('stopwords')"

Stanford parser (bash commands -- very large, consider downloading after talk):
    wget http://nlp.stanford.edu/software/stanford-corenlp-full-2015-12-09.zip
    unzip stanford-corenlp-full-2015-12-09.zip

    git clone https://github.com/brendano/stanford_corenlp_pywrapper
    cd stanford_corenlp_pywrapper
    pip install .
    cd ..

Code using these modules:
https://github.com/MSeal/kdd2016

# Docs
* Overview Slides: https://docs.google.com/presentation/d/1d7KWc3_R4s7qwTfALx2umA6WOIZbnfDJppYcqLflQug/edit
* Tutorial Slides: https://docs.google.com/presentation/d/1IBGxd9bbQ4ap5Hcd1dllavW8ZNIGbN8luXC5xOgDJUc/edit#slide=id.g15e666b122_0_0
* AWS EMR: https://docs.google.com/document/d/14lF3GZoWHoe0CkdViCcWa6fE_92sIvgOarsQQJg7ckY/edit
* AWS Lambda: https://docs.google.com/document/d/1Gw9SkHNisT6uogYEVqBWIys1tPLFVm6_y2MrMOoOU6g/edit

# Overcoming the AWS Lambda 5 minute limit
* https://serifandsemaphore.io/aws-lambda-going-beyond-5-minutes-34e381e71231?gi=a2bf8ded66e0#.wnzp1aog1
* https://aws.amazon.com/blogs/compute/better-together-amazon-ecs-and-aws-lambda/
