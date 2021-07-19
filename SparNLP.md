# Spark NLP

        Spark NLP is an open-source natural language processing library and build on top of Apache spark and Spark ML. It has two algorithms:Entity Recognition and Information Extraction. It has two contents: Sentiment Analysis and Document Classification.

## Spark ML Pipeline

* The ML-pipeline is a High-level API for MLlib that lives under the spare ml package. A pipeline consists of a sequence of stages. There are two basic types of pipeline stages: Transformer and Estimator. A Transformer takes a dataset as input and produces an augmented dataset as output.

* A pipeline is specified as a sequence of stages, and each stage is either a Transformer or an Estimator. These stages are run in order , and the input DataFrame is transformed as it passes through each stage. For the transformer stages, the transform method is called on the DataFrame.

## Annotation Format

 * Annotation 
   
   * annotationType
   * begin
   * end
   * result
   * meta-data
   * emeddings

 * AnnotatorType

   * Input: setInputCols()

   * Output: setOutputCol()

   * Approach: fit()

   * Model: transform()

## Embedding in Spark NLP

* text embedding converts text words or sentences into a numeric vector

* text embedding methods encode words and sentences in fixed length dense vectors to drastically improve the processing of textual data.

