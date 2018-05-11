---
layout: post
title: (Yet another) Introduction to Supervised Learning
---
# Motivation
Machine learning is all the rage today, and for good reason. We as humans have a lot of data that we output. From the basics of spending that our credit card companies know about to the heart rate monitoring data that my watch collects. We provide a lot. Machine learning helps us make sense of all that data and not be overwhelmed by it. For example, it allows us to know if the spike in my heart rate was the result of me going on a long walk, or because I just got into an argument about something stupid. Anyway if you're looking at this page, likely you already know this. So lets get started.

Supervised learning is a subset of machine learning. Specifically, supervised learning is the process by which we can feed a computer information about the relationship between two things (e.g. my heart rate data, as well as self reports on the activities I was doing at the time), in order to then feed the computer part of the data and have it figure out the other part. The idea is that if I have my Apple Watch (ooohh...pretty) track my heart rate at all times, while also telling it when I'm doing activities (for example if I'm running I'll let it know), then it'll develop a good idea of my average heart rate, the variability in it, etc. That's great!

![Apple Watch](/images/aw.jpg){: .center-image}

Here's the cool part. Lets go ahead and assume now that your watch notices that your average heart rate is approximately 65 bpm (nice). The coolest situation here would be if your watch kept an eye on you. How so? Well specifically let's say that you haven't been moving around much in the last hour because you're at work, and your heart rate spikes to 100 bpm. Given the previous information, your watch now (given the capability) connect the dots to say that hey, you might be having a heart attack!


Now that have have the motivation out of the way, lets figure out how to allow your watch to connect the dots.

# The Actual Introduction
We have quite a few terms to go over, and here's one of them: **predictors**. Predictors are in fact the things that you put into the model. In the case of our watch, we would be putting in the heart rate, as well as a binary of whether we're working out. The output of the model is then called the **responses**. Basically, you have your independent variables, and your dependent variables.


For all variables, we also tend to have variable types. What I mean by this is basically how we're presented the information. In our previous example, we were looking at heart rate and presence of exercise. In that case then we have a quantitative variable (the heart rate), we have the categorical variable (the exercise) as inputs, and the output type here is also categorical (are you having a heart attack).

We can call what we're doing (outputting a categorical variable) a **classification task**. Another output might be a **quantitative task** (e.g. if you want to predict the temperature on a certain day).

From now on, we're going to start denoting the input variables as $X$. Keep in mind, you'll have $X$ as a vector most of the time, so you can refer to particular inputs as $X_{j}$. The outputs are a bit different. If we have an output that's quantitative we'll denote it as $Y$, if the output is qualitative we'll denote it as $G$. With a matrix, we can denote it with a bold letter: $\textbf{X}$. Why am I telling you this? Because here's what our example is going to look like:

> Given an input vector $X$ we want to make a prediction of $G$

How can we do that? Find out next time on, machine learning learning!
