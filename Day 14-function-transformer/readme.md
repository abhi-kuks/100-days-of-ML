# ***[Function Transformers In-Depth Understanding Notebook](https://www.kaggle.com/code/abhikuks/function-transformer-in-depth-understanding/notebook)***
> Basically, these are mathematical transformations that we implement on columns to make data normally distributed.
What is so special about normal probability distribution? Why do so many data science and machine learning articles revolve around normal probability distribution?

***A Little Background First***

- Firstly, the most important point to note is that the normal distribution is also known as the Gaussian distribution.
- Secondly, it is named after the genius of Carl Friedrich Gauss.
- Lastly, an important point to note is that simple predictive models are usually the most used models. This is due to the fact that they can be explained and are well-understood. Now to add to this point; normal distribution is simple and hence its simplicity makes it extremely popular.

***What Is Normal Distribution?***

A normal distribution is a distribution that is solely dependent on two parameters of the data set: the mean and the standard deviation of the sample.

> - Mean — This is the average value of all the points in the sample that is computed by summing the values and then dividing by the total number of the values in a sample.
> - Standard Deviation — This indicates how much the data set deviates from the mean of the sample.

    This characteristic of the distribution makes it extremely simple for statisticians and hence any variable that exhibits normal distribution is feasible to be forecasted with higher accuracy. Essentially, it can help in simplifying the model.
    
***How to find if the data is normally distributed or not ?***

- we can use seaborn's sns.kdeplot
- pandas pd.skew() and pd.kurt() to check skewness and kurtosis of distribution.
- QQ Plot 

## Function Transformer has different types to make data more normally distributed
> 1. ***Log transformer*** 
    - mostly used on right-skewed data.
    - It cannot be applied to negative data as we can't calculate the log of negative numbers
    - It helps in the accuracy of linear models as it changes the additive scale to multiplicates scale.

> 2. ***Reciprocal*** 
    - It is mostly used when we need to change small values to big values and vice versa

> 3. ***Square***
    - Mostly used in left-skewed data

> 4. ***Squareroot***

> 5. ***Custom Transformation*** 
    - We can make our own transformations
## Everything Implemented in this ***[Notebook](https://www.kaggle.com/code/abhikuks/function-transformer-in-depth-understanding/notebook).***

# Thanks for giving it a read !!
