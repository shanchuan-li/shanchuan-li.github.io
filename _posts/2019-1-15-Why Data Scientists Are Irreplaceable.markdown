---
layout: post
title:  Why Data Scientists Are Irreplaceable
description:
img: Data-Scientist.png
date:   2019-01-15 01:30:00 +0200
categories: jekyll update
---
A few days ago, a friend asked me an interesting question:” I took an elective in machine learning, and according to my experience, with tools such as Scikit learn, most of the machine learning models can be trained with just a few lines of codes. Then what would be the value of a data scientist to the company if there’s a standardized tool created that everyone can learn to use, with an interface similar to Microsoft Office in the near future?”

This is similar to a question that I also had myself when I first got in touch with data topics two years ago. When I was taking the machine learning specialization on Coursera.com, there were always two assignments came with a session, one asking you to specifically code the backend of the algorithms, using gradient descent to reach the minimum of different loss functions. The other one just requires simple implementation of a model using “one line of code” and then evaluate and visualize it with another few lines. So I was wondering why do we need to learn algorithms the way that Computer Science students study them if there are already packages existing.

After two years of hands-on experience and more research, now I am able to provide an answer to this question. There are plenty of examples of why libraries are good because they really are, and the final solution that a data scientist provides for the client or his/her company, the best implementation, is unlikely to be the algorithm that he/she writes from scratch, even if he/she is a really good developer. But there is still a need to learn the algorithms if one wants to pursue a career in data science, and here is why:

Even when we’re relying on packages in our daily work, deploying a machine learning model is a process, during which a lot of questions should be answered if we want to improve the performance of the initial model: Have we implemented the best feature engineering and feature selection methods that are suitable for the dataset as well as the algorithm; Have we used the right objective function that works in our case; Do we need further parameter tuning; What does each parameter mean, and how should we tune them, such as the penalty parameter, max depth of the tree, and the learning rate; Does the evaluation metric for the validation set fit the business need, and is the validation methodology robust.

When we leverage high-level packages to perform actions, the power we have over these algorithms reduces, and consequently, the responsibility on the user is lower, making the code less error-prone. But there are in rare cases that we need an implementation of an algorithm that is not yet available in libraries, for instance - the [Import Vector Machines][IVM documentation], an algorithm I just heard recently. So this is when we need more flexibility by having to code the algorithm especially when the algorithm suits well to our dataset. 

Finally, if a data scientist is more on the “machine learning engineer” side, working with lower level packages such as TensorFlow and Keras to implement deep learning models, an understating of the lower level math and theories becomes more essential. And we have to admit in this we normally learn better by coding rather than just reading when it comes to the math and theories.

To sum up, it is still a common practice to use built packages while implementing machine learning models, and people who actually end up coding their own algorithms are researchers in universities or Google and Kaggle challengers. But coding from scratch is definitely not redundant, instead it is one of the most valuable parts of data science education, since it improves our understanding of the algorithms, and without the understanding we can't confidently interpret the intermediate results or reliably choose the next course of action towards improving the results during the model deployment process.

Referring to the question in the first paragraph, even if there are more interactive platforms created, a data scientist is still irreplaceable because of the education and knowledge that cannot quickly mastered by the newcomers, and these understandings are essential when using the tool. And actually there is already more intuitive software now available in the market, such as Rapidminer, but will this be the trend of data science in the upcoming years and replace programming languages? I will discuss this in the next post.

[IVM documentation]: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4829386/