# theiconictechnical
Technical Project for TheIconic

Notes:

For Question 3 in the SQL file, I used the OR command to find the three categories of orders made, I am aware the OR command in SQL can act up sometimes. A better way to do this would have been to create 3 temp tables and union them then select distinct account number and average revenue over the union, however OR seems to work in this case
For Question 4 in the SQL file I made the assumption that we would e-mail only those who had purchased male items before and spent >= $1000, I am not an expert on marketing strategy and would ideally like to consult others when deciding how to roll out a campaign but made the most logical decision I could come up with
I converted the original JSON data to CSV format before loading into R, simply because R works better with CSV files and it saved a lot of time doing data cleaning/manipulation
In my R markdown code, I do a quick and easy inference of gender mainly because I ran out of time. I used a simple logical if male_items > female_items then "Male" else "Female", ideally I would have used a k-means on 30% of the data containing only gender specific columns and then predicted the gender on the remaining 70% to protect from data leakage. Then using the remaining 70% of the data I would train and test a neural network on a further 70/30 split of the 70% of data which the flag was predicted on
As mentioned above, because I inferred gender so simply there is data leakage. My neural network achieves a high accuracy likely because the initial split is simply based on Male_items vs. female_items. 
