# Research on attitudes of Singaporeans towards both China and the United States.
Objective: The analysis aims to shed light on the nuanced views of Singaporeans and uncover any intriguing trends within the data towards the two nations from the Pew Research Center.

# Importing Data from SPSS to R
Since the data obtained is in SPSS format, the Haven package was used to import in the dataset. It was then named as "attitude" in a dataframe format. <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/199dd782-cbd2-4bed-a274-d9fa24e2db7d)

# Data Exploration and Cleaning
<img width="748" alt="image" src="https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/f001af83-87ae-42ba-ad25-68da7f87f149">
1. In the dataset, the countries are labelled using numbers. To check for Singapore, the unique command was used and it's tied to number 14. Therefore, a subset is created for all survey questions related to Singapore. <br>
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/bdd821f3-11df-4988-9b02-0b127f017473)

2. There are 351 survey questions in total. To look through the questions, the names() and unique() commands were used. In total 6 questions were picked. The 6 relevant variables were put together and a new dataframe was created with sg.fil.attitude. 2 pairs of variables were picked because of the ability to conduct direct comparisons and visualize as the questions are the same. The 2 pairs are fav_us and fav_china, and growinflu_us and growinflu_china. 
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/7caba3e7-4f4e-4a7e-8850-2d0d94e1a70a) <br>

3. Filter to show only Singapore's responses to the 6 variables. The clean dataset is ready to be visualised.
![image](https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/edb88c46-0a49-4c55-a669-95f4aa7c7e0e)
<img width="1117" alt="image" src="https://github.com/Kfkyyian1/pewresearchcenter_springsurvey2022/assets/146427900/0b816f36-fe9b-4c5f-a9c8-7c3afe293bd9">

# Plot 1: 


