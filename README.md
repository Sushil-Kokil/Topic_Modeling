# Topic-Modeling
Using scikit-lean done Topic Modeling with the help of the NMF, LDA 

## Comparison between NMF, LDA. Under what situations should we choose LDA or NMF?
Latent Dirichlet association (LDA) and Non-negative matrix factorization (NMF) are extensively used by Data modelers and widely accepted in scientific community for topic extraction. LDA is a probabilistic model and NMF is a matrix factorization and multivariate analysis technique.
### Latent Dirichlet Allocation (LDA)
  - Assumes each document has multiple topics
  - Works best with longer text such as full articles, essays, and books.
  - Evolves as you process new documents with the same model.
  - Results are not deterministic, meansing you might get different results each time for the same data set.
### Non-negative Matrix Factorization (NMF)
  - Calculates **how well each document fits each topic**, rather than assuming a document has multiple topics.
  - Usually faster than LDA, because of numpy array.
  - Works best with shorter text such as tweets or titles, or questions.
  - Result are deterministic, having more consistency when running the same data.


## Dataset 1: The articles from NPR (National Public Radio), obtained from their website www.npr.org
Data has contains 11992 articles.
K number of topics in LDA and NMF depends on the intution on the dataset. I consider the 7 document. I tried mutiple values for this. Finalize the 7 topics for LDA and NMF

## Dataset2 : For this project I will be working with a dataset of over 4,00,000 quora questions that have no labeled cateogry, and attempting to find 20 cateogries to assign these questions to. 

## Pre-processing
- For LDA - using CountVectorizer
- For NMF - using TfidfVectorizer

## Topic Modeling
- Using LDA and NMF
- In LDA we find the topics for the documents based on the words catergorization and documents classified on the topics, topics are assigned to each article based on the greater probability of the topics.

- In NMF we find the the coefficient of realtion of the topics to each document and assign the topics which has more coefficient.
- Also we can give the topic model name: It is depend on us that if we want to make that easy to understand or have some domain Knowledge.


![image](https://user-images.githubusercontent.com/83071381/146671377-1a2a6a9a-0e80-4629-bfd0-7ae07ddf5c40.png)
![image](https://user-images.githubusercontent.com/83071381/146671433-56106a70-a318-4670-a289-5d8b0394ac45.png)
