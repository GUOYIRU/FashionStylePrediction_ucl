# Project: Fashion Style Prediction

## Install
This project requires Python and the following Python libraries installed:

NumPy
Pandas
matplotlib
scikit-learn
spacy
xgboost
nltk
gensim
asyncio

You will also need to have software installed to run and execute a Jupyter Notebook

To see the detailed package installations, please use requirementst.txt and run code below in terminal:
-> pip install -r requirements.txt

If you do not have Python3 installed yet, it is highly recommended that you install the Anaconda distribution of Python3, which already has the above packages and more included.

## Code
DataCleaning.ipynb -- Data Cleaning includes useful information filtering; clothes categories filtering; removing of html formats, digits, punctuations etc.

DataPreprocessing.ipynb -- removing stop words, tokenizition and lemmatization.

DataLabelling.ipynb -- labelled data with pre-defined style-brand lists by LCF groups as well as manually labelled by using Labelbox.

TFIDFs.ipynb -- use gensim to get tfidf vectors to weight the embeddings as well as been used to train on the model directly.

Word2Vec.ipynb -- use gensim to get word2vec embeddings with different dimensions, and use tfidf vectors to weight the embeddings. The description embeddings are represented as averaging weighted word embeddings.

Doc2Vec.ipynb -- use gensim to get document/description veoctors directly.

FastText.ipynb -- use gensim to get fastText word/term embeddings, and then use weighted word embeddings (by tfidf) to represent description embeddings.

pretrainedembeddings.ipynb -- use pre-trained word embeddings by googlenews to represent descriptions.

kmeans.ipynb, kmeans_nap.ipynb, kmeans_nap_googlenews.ipynb -- use kmeans clustering algorithms to cluster the descriptions embeddings.

dissimilar_desc_kmeans.ipynb -- use the clustering results to find the most dissimilar products/styles

PseudoLabelling.ipynb -- use pseudo labelling to give approximate labels based on the basis of labels.

multilabel.ipynb -- use the approximate albels to do multi-label classifications.

## Run
In a terminal or command window, navigate to the top-level project directory boston_housing/ (that contains this README) and run one of the following commands:

ipython notebook notebookname.ipynb
or

jupyter notebook notebookname.ipynb
This will open the Jupyter Notebook software and project file in your browser.

## Data
Data used in this project is scraped from shopstyle.com, net-a-porter.com, farfetch.com.
