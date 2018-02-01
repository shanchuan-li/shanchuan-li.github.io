---
layout: post
title:  " Scikit-learn vs. Spark MLlib: Comparison Between Two Popular Machine Learning Frameworks"
description: You will find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes.
img: mllib-v-spark.jpg
date:   2018-01-31 21:30:52 +0200
categories: jekyll update
---
In my first post, I'd like to talk about two machine learning frameworks that I¡¯ve been using: Scikit-learn and Spark MLlib. We know that Scikit-learn is run on Python, but Spark MLlib runs within the framework of Spark, which can be written in Python and Scala. However, since Spark is written in Scala, the MLlib API runs faster in Scala than Python(pyspark). But it is obvious that Python is more popular and easier to learn. Pyspark is also popular since Python provide us with other mature data-processing libraries such as Pandas. Overall, for large datasets, using Spark¡¯s distributed computing should be much faster than using a single machine. Moreover, Spark fits well into HDFS (Hadoop Distributed File System). 

Python and Scikit-Learn do in-memory processing and in a non-distributed way, and since it has been launched for a long time, Scikit-learn can achieve more functions such as hyper-parameter optimization. Besides, since Scikit-Learn fit well into IDE such as Jupyter Notebook, it is much more powerful in in-process visualizations. However, although there are IDEs such as Apache Zeppelin embedded in cloud computing framework, for example, AWS (Amazon Web Services), in most cases we use pyspark in a Linux terminal, which does not support visualization.

Overall, MLlib has a great potential but is still in development. It now includes pre-processing that works within the Spark framework. Scikit-learn supports ¡°pipeline¡±, which provides a shortcut for data mining process, so now we have a package based on MLlib: Spark ML that supports Dataframe and pipeline. Let¡¯s say that if the machine learning packages (MLlib and ML) within Spark is as sophisticated as Scikit-Learn, maybe big-data-driven companies would use Scikit-Learn as a tool to build prototype models, and finally implement the model in Spark, just as the way Python has been replacing R in the past few years.

Check out the [Scikit-Learn Documentation][scikit-learn], [Apache Spark MLlib][spark-mllib], and [Apache Spark ML][spark-ml] for more information. 

[scikit-learn]: http://scikit-learn.org/stable/
[spark-mllib]: http://spark.apache.org/mllib/
[spark-ml]: https://spark.apache.org/docs/1.2.2/ml-guide.html
