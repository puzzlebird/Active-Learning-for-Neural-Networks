# Active-Learning-for-Neural-Networks
This re-implemented the "EGL-word" method proposed in AAAI 2017 paper ["Active Discriminative Text Representation Learning"](https://arxiv.org/pdf/1606.04212.pdf) in Tensorflow (the original implementation was in Theano). It compared the "EGL-word" method with two baseline methods "random" and "entropy" on a sentiment analysis dataset.

First run "python process_data.py path/to/pre-trained-embedding" to generate the processed data.

Then run "python active_learning.py --AL_method=active-learning-method", where "active-learning-method" should be one of "random", "entropy" or "EGL".

The following figure is the average learning curve over five runs of 10-fold cross validation. 

![Learning Curve](https://github.com/yezhang-xiaofan/Active-Learning-for-Neural-Networks/blob/master/results.png)
