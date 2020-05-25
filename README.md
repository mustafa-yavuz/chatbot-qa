# End-to-end memory network implementation for Question answering
This is an implementation of a chatbot that can answer questions based on a "story" given to the bot.

### Dataset
* [Babi](https://research.fb.com/downloads/babi/) dataset released by facebook research.
* A particular subset of the dataset which has stories, questions and answers is used as data.
* Training set(10000) and test set(1000) are seperated and each sample is in a tuple format (story,question,answer)

### Model
<img src='https://i.imgur.com/0YVe2dY.png' title='Poster' width='' />

The model takes a discrete set of inputs **x1, ..., xn** that are to be stored in the memory, a query **q**, and
outputs an answer **a**. Each of the **x**, **q**, and **a** contains symbols coming from a dictionary with **V**
words. The model writes all x to the memory up to a fixed buffer size, and then finds a continuous
representation for the **x** and **q**.



