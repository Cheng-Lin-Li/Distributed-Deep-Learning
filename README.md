# Distributed_Deep_Learning
Distributed Deep Learning with Apache Spark and Keras

This is my personal research on distributed LSTM computing with Apache Spark with Keras / Tensorflow or scala with Deep4j.
The data is time series of Dow Jones stock market price.

## Dataset

Target: 30 stock symbols from Dow Jones.
Time frame: Sep. 29, 2016 to Sep. 29 2017

## Experiment Models:
1. Long Short Tmer Memory (LSTM)
2. Gated Recurrent Unit (GRU)

## Distributed Model Design.
1. Data split into 2 partions 
1. Partition by Symbols. (Every 15 symbols will be trained on each network)
2. Partition by Time. (Every 6 months of data will be trained on each network)


Reference:
1. https://db-blog.web.cern.ch/blog/joeri-hermans/2017-01-distributed-deep-learning-apache-spark-and-keras
2. https://github.com/cerndb/dist-keras
3. https://github.com/cerndb/dist-keras/tree/master/examples
4. https://www.slideshare.net/emanueldinardo/distributed-implementation-of-a-lstm-on-spark-and-tensorflow-69787635

Scala related reference:
5. http://bayesanalytic.com/scala-fetch-stock-bar-data-from-yahoo-finance-service/
