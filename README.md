![Avatar](sample_pic/bender_hex_mini.png) 

# Encoding categorical features - comparison of several strategies, including catboost

There are plenty of methods for encoding categorical features. One of the most known is the one hot encoding. Although useful, it can be harmful for tree based models. Indeed, it's now proven that OHE biases the results towards the high cardinality features. Moreover, it increases the dimensionality, sometimes in a critical way. Therefore, it's useful to consider different methods. Hopefully, a sklearn-contrib module makes that easy.
In the dedicated section, I perform a test for Telco data. A more exhaustive benchmarking can be found [https://github.com/DenisVorotyntsev/CategoricalEncodingBenchmark](here). However, I encourage you to test the different methods, using cross-validation, on your data set or at least use the most relevant method for your data (some of them have specific assumptions and restrictions). This is a fork of a script written by Will mcGinnis

**References**:
 - [sklearn-contrib categorical encoders](https://contrib.scikit-learn.org/categorical-encoding/)
 - [https://catboost.ai/docs/concepts/tutorials.html](catboost) 