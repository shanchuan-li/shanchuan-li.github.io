---
layout: post
title:  "Scikit-learn vs. Spark MLlib: Comparison Between Two Popular Machine Learning Frameworks"
description: 
img: mllib-v-spark.jpg
date:   2018-01-31 21:30:52 +0200
categories: jekyll update
---
In my first post, I'd like to talk about two machine learning frameworks that I've been using: scikit-learn and Spark MLlib. We know that scikit-learn is run on Python, but Spark MLlib runs within the framework of Spark, which can be written in Python and Scala. However, since Spark is written in Scala, the MLlib API runs faster in Scala than Python(pyspark). Besides, some functions, such as Dimensionality Reduction(SVD and PCA), are currently only supported in the Java and Scala APIs, although it is obvious that Python is more popular and easier to learn. Pyspark is also popular since Python provides us with other mature data-processing libraries such as Pandas. Overall, for large datasets, using Spark's distributed computing should be much faster than using a single machine. Moreover, Spark fits well into HDFS (Hadoop Distributed File System). 

Python and scikit-Learn do in-memory processing and in a non-distributed way, and since it has been launched for a long time, scikit-learn can achieve more functions such as hyper-parameter optimization. Besides, since scikit-learn fits well into IDE such as Jupyter Notebook, it is much more powerful in in-process visualizations. However, although there are IDEs such as Apache Zeppelin embedded in cloud computing framework, for example, AWS (Amazon Web Services), in most cases we use pyspark in a Linux terminal, which does not support visualization.

Overall, MLlib has a great potential but is still in development. It now includes pre-processing that works within the Spark framework. Scikit-learn supports pipeline, which provides a shortcut for data mining process, so now we have a package based on MLlib: Spark ML that supports Dataframe and pipeline. Let's say that if the machine learning packages (MLlib and ML) within Spark is as sophisticated as scikit-learn, maybe big-data-driven companies would use scikit-learn as a tool to build prototype models, and finally implement the model in Spark, just as the way Python has been replacing R in the past few years.

Check out [Scikit-Learn Documentation][scikit-learn], [Apache Spark MLlib][spark-mllib], and [Apache Spark ML][spark-ml] for more information. 

[scikit-learn]: http://scikit-learn.org/stable/
[spark-mllib]: http://spark.apache.org/mllib/
[spark-ml]: https://spark.apache.org/docs/1.2.2/ml-guide.html
