# Introduction to Data Mining

### Repository Information and About Me ###
This is the Gitlab page for my work in Introduction to Data Mining. <br>

My name is Qixiao Zhu and you can call me Jimmy.
I am double majoring in Computer Science and Music with a 
piano performance concentration. I love to code and learn
about computer science. At the same time, I do a lot of projects
related to augmented reality, audio processing, and music software development. <br>

I wish to learn a lot about data science in this course, and I am really looking
forward to learning different models of machine learning. I am extremely passionate
about machine learning and data science and want to get more familiar with them.

### Final Project Information ###
Final Project Report Video: https://youtu.be/w0oFfmKs6rs <br>

The final project uses the dataset "Glass Identification Data Set" from the 
UCI Machine Learning Repository: http://archive.ics.uci.edu/ml/datasets/Glass+Identification
to hone and test my skills in data mining and machine learning through predicting the type
of glass each instance represents using neural network. <br>

This dataset is hard to deal with because it has imbalanced classes and it does not have a lot 
of samples. Because of this characteristic, I tried multiple methods to train decent neural network
classification models. <br>

In my later experiments with different methods of coping with this imbalanced dataset, I have
found that this dataset was unexpectedly hard to fit a classification neural network. Different
classes had different numbers of samples. The largest class had 76 elements, while the smallest
class only had 9 elements. At first, I chose to simply use the weighted f1 score as 
the performance metric, but it only had a score of 70% when using cross validation. I  then tried 
to use an oversampling technique called SMOTE, which generates samples for the smaller classes so
that each class had the same number of samples, and I used accuracy for the performance metric after
oversampling. It resulted in much better scores, with about 90% accuracy when doing cross validation.
After I tuned the hyperparamenters, I tried to split the original data, train with oversampled data, 
and test with the portion that is not oversampled. Train test split test resulted in about 75% accuracy. 
I had to adjust the number of epochs a little to prevent overfitting on the oversampled training data. 
The result was not a particularly satisfying one, but it was the first time I have dealt with 
imbalanced data and the progress from not even close to accurate to somewhat accurate predictions was 
satisfying for me.