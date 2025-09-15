# Student Stress and Academic Performance (Data Mining Project 1)
<b></b>
<H2>Introduction to the Problem</H2>
<b>For this project I picked the student stress monitoring dataset. The dataset explores the cause of student stress in college students between the ages of 18-21 all across the United States. This dataset is based off the responses of 843 different college students across the country, the survey contained 25 different questions and student responses were condensed into 20 different key features that are grouped into 5 main categories: Psychological factors, Physiological factors, Environmental factors, Academic factors, and Social factors. My hope is to figure out which factors most impact stress levels and which category holds the most impact on the daily life of college students in the United States.</b>
<b>I also hope to find a practical use where a university or even students themselves can have a tangible way to see if controllable factors in their life, like sleep quality can make an effect on their stress levels. I see there is also a column for academic performance that students and universities can use this data in order to boost academic performance. I could also imagine universities using this data to see if there is a way they can better help assist their students to fight stress and boost student well being effectively.</b>
<h2>Pre-processing the Data</h2>
<b>The data was already free of nulls when I first opened it however I still made sure the column names were consistent and checked for other errors in consistency. I did this by loading the csv file (StressLevelDataset.csv) into pandas and did a few checks.</b>
<ul>stress_df_clean = stress_df.dropna()
print(stress_df_clean) </ul>
<b>For the most part the data was numerical and formatted in a way that works for me. This dataset was ready for analysis and visualization.</b>
<h2>Data Understanding/Visualization</h2>
<b>Once my dataset was cleaned up I started looking for trends and patterns as well as just explored the dataset by comparing different variables.</b>
<b>The heatmap visualizes the correlation between all numeric variables in the dataset. Darker or lighter cells indicate stronger positive or negative associations. This helps identify which factors appear most strongly linked with stress.</b>
<img width="980" height="830" alt="download" src="https://github.com/user-attachments/assets/479e09aa-016d-4c22-96c3-afb60c2b821e" />
<b>Here we’ve grouped individual variables into the 5 broad categories discussed psychological, physiological, environmental, academic, and social. I then calculated each category’s average correlation with stress. The bars show which domains contribute most to stress, making it easier to see patterns at a higher level.</b>
<img width="790" height="590" alt="download" src="https://github.com/user-attachments/assets/11f4805f-6655-409e-bca1-5b2440bd3e4e" />
<b>This scatter plot with a regression line shows the relationship between sleep quality and stress level for all students. The downward slope indicates that, on average, students with better sleep quality tend to report lower stress.</b>
<img width="650" height="500" alt="download" src="https://github.com/user-attachments/assets/bc015a5d-ac1a-4895-813b-d35f81b5e6af" />
<b>In the combined plot, each academic performance group is shown in a different color, with its own regression line. This allows direct comparison of how the sleep–stress relationship differs across performance levels in a single view.</b>
<img width="650" height="465" alt="download" src="https://github.com/user-attachments/assets/bd3f454c-0878-4fc6-b338-c3b4cbef16e6" />
<b>In the faceted version, the same relationship is plotted separately for each academic performance group. This removes overlap and makes it easier to see within-group trends without distraction from other groups.</b>
<img width="2690" height="1000" alt="download" src="https://github.com/user-attachments/assets/6137f4f1-44e2-45fe-b300-5f4a3c4be1d0" />

<h2>Storytelling/Findings</h2>
<b>After analyzing my data, I found several relevant takeaways. From the heatmap, I was able to identify the individual factors that have the strongest direct effect on stress_level. Bullying showed the highest Pearson correlation coefficient at 0.75,followed closely by future_career_concerns(0.74), anxiety_level(0.74), and depression(0.73). The heatmap provided the most in-depth individual breakdown on how students are affected by the factors relate to one another. Observing how the positive and negative correlation coefficients change highlight which factors most influence students on day to day basis 
From the category-level correlations bar chart, we can see that social stressors have the highest correlation with increased stress levels, which aligns the heatmap. The sleep_quality vs stress_level scatterplot shows a downward regression line indicating that the lower the quality of sleep, the higher the stress levels of students generally. Finally, by factoring academic performance groups we can deduce that the highest academic performing students have lower stress levels when their sleep quality is higher.   </b>
<h2>Impact</h2>
<b>add information about Impact here</b>
<h2>References</h2>
<ul>1. https://www.kaggle.com/datasets/mdsultanulislamovi/student-stress-monitoring-datasets?resource=download </ul>
<ul>2. </ul>
<ul>3. </ul>
<ul>4. </ul>
