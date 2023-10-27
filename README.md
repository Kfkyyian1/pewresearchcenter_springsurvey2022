# Research on attitudes of Singaporeans towards both China and the United States.
Objective: The analysis aims to shed light on the nuanced views of Singaporeans and uncover any intriguing trends within the data towards the two nations from the Pew Research Center.

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
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/edb88c46-0a49-4c55-a669-95f4aa7c7e0e)
<img width="1117" alt="image" src="https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/0b816f36-fe9b-4c5f-a9c8-7c3afe293bd9">

# Visualisation
Since the survey answers are categorical data, only bar charts were plotted to analyze the data. It’s the most suitable type of graph as it can compare the distribution of responses across different categories such as gender and age. 

## Plot 1 - Singapore's favor response towards the United States and China
<img width="481" alt="image" src="https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/f226797e-6da4-4a50-ab7a-f6c8a2b8f88d"> <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/b8643ab8-7e00-43a1-8657-6d28ec5beb1c) <br>
Overall, Singapore’s response towards these two countries is quite similar. Majority of them are somewhat favorable with the respective countries. However, when we combine the favorable responses and compare it with total unfavorable responses, Singapore is leaning towards favoring China more than the United States. Notably, a larger proportion of respondents expressed "Somewhat Unfavorable" or "Very Unfavorable" opinions towards the United States compared to China.

## Plot 2 - Responses towards the United States by age
To gain deeper insights, respondents' ages were categorized into groups and added to the analysis. Age groups were defined using the "cut" function and incorporated into the box plots for both countries. <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/09420e73-ecbf-41f3-96d4-aa360893e1df) <br>
<img width="452" alt="image" src="https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/44ce63eb-a1d9-4556-8cfa-1665e2c85459"> <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/40e001e6-6230-4370-b732-b788739a33fa)
Majority of the respondents who expressed “Somewhat Favorable” are within the age of 25-44. However interestingly, both the same age groups are the highest in expressing that they are “Somewhat Unfavorable”. It seems the 35-44 age group is divided almost evenly between both responses. By looking at “Very Unfavorable”, almost all age groups have the same thoughts except those under 25 and above 74. Similarly, the box plot in Exhibit 7 was also created for China below.

## Plot 3 - Responses towards China by age
<img width="452" alt="image" src="https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/61b5561a-6708-4581-8c95-549c1420c6d8"> <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/a138d93c-d2ae-4e7a-a9f9-02114ae70167) <br>
The ratio of age groups who expressed “Somewhat Favorable” and “Somewhat Unfavorable” towards China are almost identical to the United States, age 25-44 make up most of the count. Those who are “Very Unfavorable” decrease as the age increases from 25 – 84. Another interesting observation is that those within 25-34 and 45-54 are “Very Favorable” towards China. In the United States, 45-54 had the most respondents within this response. 

## Plot 4 - 









