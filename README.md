# Research on attitudes of Singaporeans towards China and the United States.
Objective: The analysis aims to shed light on the nuanced views of Singaporeans and uncover any intriguing trends within the data towards the two nations from the Pew Research Center. 

* Note: Raw data was obtained from from https://www.pewresearch.org/global/dataset/spring-2022-survey-data/

# Importing Data from SPSS to R
Since the data obtained is in SPSS format, the Haven package was used to import in the dataset. It was then named as "attitude" in a dataframe format. <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/199dd782-cbd2-4bed-a274-d9fa24e2db7d)

# Data Exploration and Cleaning
<img width="748" alt="image" src="https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/f001af83-87ae-42ba-ad25-68da7f87f149"> <br>
1. In the dataset, the countries are labelled using numbers. To check for Singapore, the unique command was used and it's tied to number 14. Therefore, a subset is created for all survey questions related to Singapore. <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/bdd821f3-11df-4988-9b02-0b127f017473)

2. There are 351 survey questions in total. To look through the questions, the names() and unique() commands were used. In total 6 questions were picked. The 6 relevant variables were put together and a new dataframe was created with sg.fil.attitude. 2 pairs of variables were picked because of the ability to conduct direct comparisons and visualize as the questions are the same. The 2 pairs are fav_us and fav_china, and growinflu_us and growinflu_china. <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/7caba3e7-4f4e-4a7e-8850-2d0d94e1a70a) <br>

3. Filter to show only Singapore's responses to the 6 variables. The clean dataset is ready to be visualised.
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/edb88c46-0a49-4c55-a669-95f4aa7c7e0e) <br>
<img width="1117" alt="image" src="https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/0b816f36-fe9b-4c5f-a9c8-7c3afe293bd9">

# Visualisation
Since the survey answers are categorical data, only bar charts were plotted to analyze the data. It’s the most suitable type of graph as it can compare the distribution of responses across different categories such as gender and age. 

## Plot 1 - Singapore's favor response towards the United States and China
![Singaporeans' Fav Towards US   China](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/fcd4909a-3182-4b02-ba67-a724324e6949) <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/b8643ab8-7e00-43a1-8657-6d28ec5beb1c) <br>
Overall, Singapore’s response towards these two countries is quite similar. Majority of them are somewhat favorable with the respective countries. However, when we combine the favorable responses and compare it with total unfavorable responses, Singapore is leaning towards favoring China more than the United States. Notably, a larger proportion of respondents expressed "Somewhat Unfavorable" or "Very Unfavorable" opinions towards the United States compared to China.

## Plot 2 - Responses towards the United States by age
To gain deeper insights, respondents' ages were categorized into groups and added to the analysis. Age groups were defined using the "cut" function and incorporated into the box plots for both countries. <br>
![Singaporeans' Fav Towards US by Age](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/120fb43c-b285-4e1b-b46f-fdb342225c54) <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/40e001e6-6230-4370-b732-b788739a33fa) <br>
Majority of the respondents who expressed “Somewhat Favorable” are within the age of 25-44. However interestingly, both the same age groups are the highest in expressing that they are “Somewhat Unfavorable”. It seems the 35-44 age group is divided almost evenly between both responses. By looking at “Very Unfavorable”, almost all age groups have the same thoughts except those under 25 and above 74. Similarly, the box plot in Exhibit 7 was also created for China below.

## Plot 3 - Responses towards China by age
![Singaporeans' Fav Towards China by Age](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/a1370ae1-3323-4084-880f-023dc03c45bf) <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/a138d93c-d2ae-4e7a-a9f9-02114ae70167) <br>
The ratio of age groups who expressed “Somewhat Favorable” and “Somewhat Unfavorable” towards China are almost identical to the United States, age 25-44 make up most of the count. Those who are “Very Unfavorable” decrease as the age increases from 25 – 84. Another interesting observation is that those within 25-34 and 45-54 are “Very Favorable” towards China. In the United States, 45-54 had the most respondents within this response. 

## Plot 4 - Favorable Comparison towards the United States and China by Gender
![Singaporeans' Fav Towards US   China by Gender](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/b3c2237b-637f-46e5-ba06-e19b8b24ca00)<br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/72e0ec7f-2030-4bfa-9ccb-b0047274fb48) <br>
Next, the favorability was also observed by gender in Exhibit 8. On majority of the responses towards both United States and China, male respondents were higher than female respondents. To conclude the favorable comparison, despite Singapore’s response towards these two countries is quite similar, but overall, it is more favorable towards China. Among the respondents, majority of them are within the age of 25 - 44 and consisted of more males. 

## Plot 5 - Singaporeans' Perceived Influence of the United States and China
![Perceived Influence of the United States and China: Singaporeans' Attitudes](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/f2f3c5f1-20b9-4855-a73f-27d252cfd408) <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/accb15d3-82d3-4a7e-b3c2-9db322161dbe) <br>
The variables growinflu_us and growinflu_china were converted to factors so that bar plots can be created. A sanity check was done using the “unique()” command. As some options were not picked by the respondents, those were removed from the box plot. Most respondents believe China's influence is growing stronger compared to the United States. This perception might be influenced by China's remarkable economic growth in recent years.
<br>
<p>
In conclusion, the analysis of Singaporeans' attitudes towards China and the United States reveals interesting findings. While Singaporeans generally hold somewhat favorable views of both countries, their perceptions of influence and favorability differ. Singaporeans view China as more influential and look more favorably upon it compared to the United States. However, it's important to note that the favorability data is heavily influenced by respondents under the age of 45, as there are fewer responses from those above 74. </p>













