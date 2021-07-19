# Gensim

## Definition

    Gensim is a tool for topic Modeling which is the process of extracting topics from large amount of documents. LDA is one of Gensim's models .

## Core Concepts

* Document-- some text
* Corpus -- a collection of documents
* Vector -- a mathematically convenient representation of a document
* Model -- an algorithm for transforming vectors from one representation to another


## Basic Methods

* Latent Semantic Analysis (LSA)
* Probabilistic Latent Semantic Analysis (pLSA)
* Latent Dirichlet Allocation (LDA)
* Correlated Topic Model (CTM)

## Topic Evolution Model

* Topic Over Time (TOT)
* Dynamic Topic Models (DTM)
* Multiscale Topic Tomography (MTT)
* Dynamic Topic Correlation Detection (DTCD)
* Detecting Topic Evolution (DTE)

## How to use Latent Dirichlet Allocation

* Step 1--choose the right library

    * Pandas-> for data manipulation and analysis

    * Gensim-> for document indexing and  similarity retrieval  in large document

    * pyLDAvis-> for interactive topic modelling visualization

    * Parivar and Huzm-> to act as an NLP library for person depending on the use case

* Step 2--Preprocess the Data
    
     * Normalization-> Transform text to normal form

     * Stemming-> Reduced a word to its word step/root without suffixes and prefixes

     * Stopwordremoveal-> Remove words that do not add any logical moving

     * Tokenization-> Break text into tokens

* Step 3-- Build the Dictionary

    * the preprocessing output text is used to build the dictionare cha corpus

    * the outputs become for the inputs for LDA models for topic modeling

* Step 4-- Select topic number through testing for Accuracy

    * A coherence matrix is used to test the model for accuracy

    * Topic coherence is a measure that compare different topic models based on their human-interpretability

    * Build many LDA models with different topic numbers, the correct model will have the highest coherence score

    * While choosing a high topic number can provide granular sub-topics, repetition of keywords indicates that the topic number is too large

    * So the correct topic value will minimize rapid increase in top coherence

* Step 5-- Visualize the Topics

    * the optimal number of topics can be better visualized through the interactive pyLDAvis tool

* Step 6-- Optimize the Topics

    * Hyperparameters are tuned to optimize the number of topics

    * Different combination of alpha(document-topic density), k(the number of topics) and beta(topic-word density) are run and their coherence scores are calculated

    * the combination with the highest coherence score is used to build the LDA Model

      
