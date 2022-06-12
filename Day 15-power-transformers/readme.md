# ***[Power Transformers In-Depth Understanding Notebook](https://www.kaggle.com/code/abhikuks/power-transformers-in-depth-understanding)***
***sklearn.preprocessing.PowerTransformer***

>class sklearn.preprocessing.PowerTransformer(method='yeo-johnson', *, standardize=True, copy=True)

> 1. ***Apply a power transform featurewise to make data more Gaussian-like (same as Normal Distribution).***


> 2. ***Power transforms are a family of parametric, monotonic transformations that are applied to make data more Gaussian-like. This is useful for modeling issues related to heteroscedasticity (non-constant variance), or other situations where normality is desired.***


> 3. ***Currently, PowerTransformer supports the Box-Cox transform and the Yeo-Johnson transform. The optimal parameter for stabilizing variance and minimizing skewness is estimated through maximum likelihood(sklearn) and is also done by Bayesian statistics but not in sklearn.***


> 4. ***Box-Cox requires input data to be strictly positive, while Yeo-Johnson supports both positive and negative data.***


>5. ***By default, zero-mean, unit-variance normalization is applied to the transformed data so don't need to apply standardization.***

## ***Observations : All practically done here in this [Notebook](https://www.kaggle.com/code/abhikuks/power-transformers-in-depth-understanding)***
> We have calculated r2 score without any power transformers, Box cox, and Yeo Johnson transformation on all the features and then plotted them as well to get the gist of it and how the data is distributed.

>## Without any 
     - r2 score: 0.6275531792314851
     - cross val score: 0.4609940491662866
>## Box-Cox Transformation 
     - r2 score: 0.8047825006181188
     - cross val score: 0.6658537942219864 
>## Yeo-Johnson Transformation
     - r2 score: 0.8161906513339305
     - cross val score: 0.6834625134285746

## ***Distribution Plots and QQ plots for each feature***
[![before.jpg](https://i.postimg.cc/vTxwF8RB/before.jpg)](https://postimg.cc/MfwF1Sp2)

## ***Before and after comparison for Box-Cox plot { Distribution Plots }***
- Left one : Before Transformation
- Right one - After Transformation
[![box-cox.jpg](https://i.postimg.cc/BbbHJyNt/box-cox.jpg)](https://postimg.cc/rR6KJfBL)

## ***Before and after comparison for Yeo-Johnson plot { Distribution Plots }***
[![yeo-johnson.jpg](https://i.postimg.cc/3rqDgtnC/yeo-johnson.jpg)](https://postimg.cc/DmqZhPV8)

# Thanks for giving it a read.
