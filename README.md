# Business-analysis-Based-on-Advertisements
这个项目主要R语言进行商业分析，收集互联网浏览者点击广告的数据，基于此来获取数据后的现象以便为后期公司决策带来帮助  
The project carries out business analysis by R language. In addition, the dataset are collected by the internet visitors clicking on advertisements. Based on the project, we can obtain the hidden phenomenon to help company make better decision in the future.  


## DataSet
The DataSet records the data of Internet Vistors who subscribe the NewYorkTime(https://www.nytimes.com/). More specifically, the information is about different background users’ clicking on advertisements during reading the news.

## Additional Library  
You need install the relevent library: ggplot2, readr, dplyr. doBy
```
require(readr)
require(dplyr)
require(doBy)
require(ggplot2)

```


## Tasks
Choose any one of days for business analysis.  
```
T1: Plot the distributions of number impressions and click-through-rate (CTR=# clicks/# impressions) for the 5 age categories as "<30", "30-39", "40-49", "50-59", "60+".  
T2: Explore the data and make visual (plotting) and quantitative comparisons (table) across user demographics <18-year-old males versus < 18-year-old females. 
T3: Create metrics that summarize the data. The metrics should include CTR, quantiles, mean, variance, and max, and these can be calculated across the various user segments.
```
Choose all days for business analysis.
```
T4: Extend your analysis across 10 days and visualize the distributions of the metrics.
T5: Describe ONE pattern you found.  
```

## Results
The nyt1 is used for business analysis.

T1:  
Young people receives more impressions than old people.    
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/the%20relationship%20between%20age%20and%20impressions.png" width ="500" height = "500">  

The male receives more impressions than female.  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/gender%20and%20impressions.png" width ="500" height = "500">  

Most of people received impressions don't click the advertisement. However, the old people prefer to click the advertisements.  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/the%20facets%20for%20the%20different%20agecats%20by%20the%20clicks.png" width ="500" height = "500">  

The people are favor to click the advertisement whose age are from 30-39 and >60.  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/CTR%20by%20age(2).png" width ="500" height = "500">  

The female prefer to click when impression more than male.  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/CTR%20by%20gender(2).png" width ="500" height = "500">  

The visitors(no signed) are likely to click when impression more than registered members(signed)  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/CTR%20by%20Signed_In(1).png" width ="500" height = "500">  

When CTR in 0.5~1.0, the young adult(<30) are likely to click when impressions. (NOTE: CTR=# clicks/# impressions)  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/CTR%20By%20agecat.png" width ="500" height = "500">  

<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/CTR%20By%20agecat_click.png" width ="500" height = "500">  

T2:  
The (<18) male and female both have same min,max and mean, but the number of male is greater than female.   
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Table/table1.png" title= "table1">  

The male and female have almost same impressions and clicks.
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Table/table5.png" title= "table5">  

The female(<18) has more impressions than male(<18)    
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/Impressions%20for%20gender(small%20than%2018).png" width ="500" height = "500">  

The number of female(<18) who become members are more than male(<18)  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/Signed_In%20for%20gender(small%20than%2018).png" width ="500" height = "500"> 

The number of female(<18) who click the advertisement are more than male(<18)   
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/scode%20for%20gender(small%20than%2018).png" width ="500" height = "500"> 

The female（<18） are more likely to click more than male（<18）when impressions.   
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/CTR%20for%20gender(small%20than%2018).png" width ="500" height = "500">   

T3:  
(Note: Now let us create new category called scode with value "NoImps", "Imps", "Clicks". And convert the column into a factor.)  
The metrics of summay for male and female in day1  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Table/table2.png" title= "table5">  

The metrics of summay for male in day1  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Table/table3.png" title= "table5">  

The metrics of summay for female in day1  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Table/table4.png" title= "table5">  

Below these three tables, it easily found the male receive more impressions and have more scode_rate than the female , but the female click more Advertisement than the male and female have strong intentions after the Advertisement pushing(reasons: CTR).  

T4:  
Male are likely to click the advertisement when working on Monday(the first day in weekdays),however the female are more focus on work on Monday.  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/gender%20for%2010%20days.png" width ="500" height = "500">  

The old people(>60) have more space time to click advertisement in all ten days, however the people(30-39/40-49) who under Career peak have low desire to click the advertisement.  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/agecat%20for%2010%20days.png" width ="500" height = "500">  

People in weekend are more likely to click the advertisement than in workday.  
<img src ="https://github.com/MinglangTuo/Business-analysis-Based-on-Advertisements/blob/master/Picture/CTR%20for%2010%20days.png" width ="500" height = "500">  

## Contribution
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)  
[xjtlu] Xi 'an Jiaotong Liverpool University
