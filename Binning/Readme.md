# BINNING

![bin](https://miro.medium.com/max/1400/0*XWta_U67Nv9udfY-.png)

Binning can be applied on both categorical and numerical data:  
1. Numerical Binning Example  

Value      Bin  

0-30   ->  Low       
31-70  ->  Mid       
71-100 ->  High  

2.Categorical Binning Example  

Value      Bin  

Spain  ->  Europe      
Italy  ->  Europe       
Chile  ->  South America
Brazil ->  South America  
  
    
The main motivation of binning is to make the model more robust and prevent overfitting. However, it has a cost to the performance. Every time we bin something, we sacrifice information and make our data more regularized.

The trade-off between performance and overfitting is the key point of the binning process.    

For numerical columns, except for some obvious overfitting cases, binning might be redundant for some kind of algorithms, due to its effect on model performance.However, for categorical columns, the labels with low frequencies probably affect the robustness of statistical models negatively. Thus, assigning a general category to these less frequent values helps to keep the robustness of the model. For example, if your data size is 100,000 rows, it might be a good option to unite the labels with a count less than 100 to a new category like “Other”.
