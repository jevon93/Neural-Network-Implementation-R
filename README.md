# theiconictechnical
Technical Project for TheIconic

Notes:

In my R markdown code, I do a quick and easy inference of gender mainly because I ran out of time. I used a simple logical if male_items > female_items then "Male" else "Female", ideally I would have used a k-means on 30% of the data containing only gender specific columns and then predicted the gender on the remaining 70% to protect from data leakage. Then using the remaining 70% of the data I would train and test a neural network on a further 70/30 split of the 70% of data which the flag was predicted on


As mentioned above, because I inferred gender so simply there is data leakage. My neural network achieves a high accuracy likely because the initial split is simply based on Male_items vs. female_items. 
