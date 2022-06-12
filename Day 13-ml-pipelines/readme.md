# ***Hello Everyone,***
***Just created a [notebook] (https://www.kaggle.com/code/abhikuks/machine-learning-pipeline-indepth-understanding) and the main goal of it is to see what happens when we work without creating the pipeline and when we work using Scikit Learn pipelines.***

[![pipeline.png](https://i.postimg.cc/FKnG6whs/pipeline.png)](https://postimg.cc/yJcFgQJw)

# So what the hell is Pipelines??

- Pipelines chains together multiple steps so that the output of each step is input to the next step.
- Pipeline makes our work easy to apply the same preprocessing to train and test.

## Still baffled ? don't worry so there are two parts in this [Notebook](https://www.kaggle.com/code/abhikuks/machine-learning-pipeline-indepth-understanding) :
- In the first half of the notebook, we'll look that how to work without any pipelines and try to kinda use them on the data.
>***why this approach is not good***
> 1. We need to follow the same process/workflow in both uat and production when we don't make pipelines.
> 2. It makes code hard to understand as updates in multiple places and hence the confusion
>3. Scikit learn comes to the rescue here that is why we should use pipelines and let's understand

- In the second half, we have used Column Transformer for making chain blocks and combining them using Scikit Learn pipelines.

>***Let's create a chain /pipeline***
>***For Each step we'll be using a column transformer and these are steps:***

>1. So now we can see that Age and Embarked got missing values -- Imputer needs to be used here because scikit learn gets angry when it sees missing values. 

>2. Sex and Embarked are Nominal categorical Values --- OneHotEncoding needs to be done because scikit learn only loves to work with numbers.

>3. We'll be scaling data so as to get everything on same scale because it helps the scikit learn attributes to understand the features with the same scale

>4. I'll be using feature selection as well just to see how it works. However, this will affect the model performance but here I want to make this as a reference to look out for how to make ML Pipeline.

>5. Now at last, we'll be using our Decision Tree Algorithm and then save the model,

***In this [Notebook](https://www.kaggle.com/code/abhikuks/machine-learning-pipeline-indepth-understanding) I'll not focus on exploring data here and model accuracy; I want you to comprehend the importance of pipelines and get the gist of it, so you have to bear with that but if you want there's a step by step basic analysis as well [here](https://www.kaggle.com/code/abhikuks/step-by-step-analysis-for-absolute-beginners) done by me.***

Thanks for giving it a read !!
