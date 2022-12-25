 👋 **Analyzing data set of users used Flood it! (English version)**
 
<!--- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...--->

<!---
ngocanhp061/ngocanhp061 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

_**Note:**_ 

*  Link of the code: https://console.cloud.google.com/bigquery?sq=127863163697:05f09145051745b29801bd809a61f8e5*

*   Link of the visualization: *https://datastudio.google.com/reporting/3381df0e-ae57-4efd-9305-2a6094642e41/page/UrP4C

Flood it! is a simple strategic game, where your mission is to flood the screen by one color in the limited time. This analysis bases on the dataset about this app’s users in the period from 12/06/2018 to 03/10/2018. The analysis will answer the following main questions:
- The number of users used the app each day
- The average hours each user used playing the app
- The average hours each user used playing the app (by countries)
- The number of users used each operating system (iOS and Android)
- The retention rate of the app (by using Cohort Analysis)
- The average sessions each day (session is the period  of time a user is active on the app, in which, the inactive period is less than 30 minutes).
- The sample dashboard to track revenue of the app

**1. The number of users used the app each day**
![image](https://user-images.githubusercontent.com/111174822/209472559-d9bb953a-9590-4d94-9d0b-910b7f16dbab.png)


The above chart illustrates the number of people used the app each day in the period from 12/06/2018 to 03/10/2018. It is easy to see that, on 18/6, 25/6, 28/6, 1/7, the amount of people tended to be higher than the other days, even 3 times higher than normal. It must be noticed that, those days are the weekdays, not even the weekends. I did some research about this game on the Internet, but it has very little information on the Internet. We can assume that on those days, the game had events to attract more users.
In fact, I did try to assume that, on those days, the game entered a new market, so it had new users. However, I observed the chart about total users used the app in each country and recognized that:
![image](https://user-images.githubusercontent.com/111174822/209472568-d665b590-3746-4a2f-8956-98ff35c74c45.png)


On all days in the 4-month period, North America was the area that had the highest amount of users. Even on 18/6, 25/6, 28/6 and 1/7 mentioned
above, North America still remained the largest player base, and nowhere had the player base increased significantly on those days.  Therefore, the assumption that the game entered a new market and caused the increase in the number of users is not suitable for this situation.
Except the days mentioned above, the remaining days had a certain number of players (ranging from 400-500 people), proving that the number of players of this app was very stable.

**2. The average hour each user used playing the app**
![image](https://user-images.githubusercontent.com/111174822/209472631-dd09c5a6-065f-444e-a135-b66caf1328b9.png)
![image](https://user-images.githubusercontent.com/111174822/209472635-15df5ebb-330b-4d42-b811-f731d44d108f.png)


The next charts illustrate the average hours each day players used to play the app. It is easy to recognize that, the average hours ranged from 2 hours to 4 hours. 18/9 was the day with the highest average hours used in a day, while the lowest one was on 6/8.
![image](https://user-images.githubusercontent.com/111174822/209472640-fcfe7380-6f55-4ee3-9ca8-0662fb7a758a.png)


In the 4-month period mentioned above, the average hours that users used per day were 2.76 hours.

**3. The average hour each user used playing the app (by countries)**
![image](https://user-images.githubusercontent.com/111174822/209472651-f65063a3-10d0-4491-a546-322b456208fb.png)


This bubble chart represents the average hours each user used to play the app in different countries. The bigger the bubble is, the higher the average hours used in that country. We can see that, the biggest bubble is in Turkmenistan, where the citizens used 11 hours per day to play the game, on average. This data can show which countries the game was popular in, to maintain the business strategy in those countries. And for countries where the game had not been used much, it is possible to expand advertising to attract people in those countries.

**4. The number of users used each operating system (iOS and Android)**
![image](https://user-images.githubusercontent.com/111174822/209472656-0412e39f-5fc3-4930-8af0-772350ccc097.png)


The number of users of each operating system is represented in the bar chart above, with the number of users of iOS and Android operating systems being almost equal. In addition, up to 1/8 of people have unknown operating system.

**5. The retention rate of the app (by using Cohort Analysis)**
![image](https://user-images.githubusercontent.com/111174822/209472659-38ceb9c6-7470-446e-aa2b-aca4a18dcfeb.png)
![image](https://user-images.githubusercontent.com/111174822/209472668-a1450ca1-e99c-4848-bd7c-d4489050f580.png)



The next chart is the heat map used for Cohort Analysis. In fact, the long-term success of application developers is not only in the number of people downloaded the app, but also in remaining the number of people continue using the app. Cohort analysis is a very useful tool to calculate the number of app users over time.
The above heat map shows the percentage of app users over time, with the darker pinks represent the higher proportion. As can be seen that, the app maintained a steady stream of returning users. In June, the rate of users returning every day was about 4-7%, but from July onwards, this rate dropped even lower, only about 2-4%. Notably, the rate of returning users on June 18 was the highest in the four months considered.

**6. The average sessions each day**
![image](https://user-images.githubusercontent.com/111174822/209472670-7f1287b1-912e-4dd2-9eb1-d0a0adcd03d8.png)
![image](https://user-images.githubusercontent.com/111174822/209472671-b336a9b4-81ee-40d8-b6d4-c13f368033df.png)




Session is defined as the period when users are active on the app. As default, if a user is inactive in more than 30 minutes, the activities after that will be counted in the new session. In other word, in each session, the inactive period must be lower than 30 minutes.
The above line graph shows the average sessions each day in Flood it! On average, there are 106 sessions per day on the app. From the end of June onward, the average sessions each day fluctuated from 75 to 150 sessions. On the other hand, the days when the number of users increased sharply (such as June 18, June 25 and June 28) had a lower number of sessions than average, with only about 50 sessions / 1 day. In fact, the average number of sessions per day is calculated using the formula:
![image](https://user-images.githubusercontent.com/111174822/209472684-f3fb252c-6e1a-4ac6-899b-9407c78a2b22.png)
![image](https://user-images.githubusercontent.com/111174822/209472698-49833d19-4cf3-4557-8be6-0f47065203ff.png)




The total sessions and total users in each day are also listed in the table above. We can see that, the total number of sessions each day are roughly the same, with about 49,000 sessions. However, days like June 18 had a much higher number of users, resulting in the average number of sessions per day falling below average.

**7. The sample dashboard to track revenue of the app**

Customer Lifetime Value (CLV) is the revenue created by users throughout their lifetime interaction with the app. For Flood it! or other free games, this revenue comes from two main sources: from advertisements and in-app purchases. The former source contributes more. So, the question for app developers is: how to track the change in revenue from the above sources?
Therefore, in this analysis, I bring the solution by this below dashboard sample.
![image](https://user-images.githubusercontent.com/111174822/209472704-28f2c34a-68fa-403e-b516-7793538f2f23.png)


This chart provides a solution to track ad impressions and ad revenue over the days. The number of ads shown was significantly high on days like June 18, June 24, June 28, September 16 (with about 50 ads). These are also the days that recorded a higher number of users than other days. The revenue from advertising was also remarkably high these days. In addition, the average number of ads that were shown per day between June 12 and October 3 was about 17 ads/day.
Two main types of costs for advertising on the app and the price of each in the Vietnamese market include:
+ CPC (Cost per click: price for 1 click on the ad): 0.03 USD/click
+ CPM (Cost per 1000 impressions: price for 1000 ad impressions): 2USD/1000 impressions, or 0.002USD/1 impression.
Revenue in the chart above is calculated using the formula: $0.002 * impressions. Flood it! app's data used in this analysis is just the sample data, so I recognized shown ads and did not recognize clicked ones. Therefore, the chart above plays a role as a sample chart, which can be similarly applied to other types of advertising.
![image](https://user-images.githubusercontent.com/111174822/209472741-4851994b-61dc-4a9b-9d77-889d338b744d.png)


There can be different products for in-app purchases, like:
+ buying a VIP package to experience limited user services
+ buying a package that doesn't show ads, etc.
The price of each of the above products is different. I also used the same chart as above to show the number of in-app purchases over the 4-month period. However, this chart does not show specific revenue, because the sample data just recorded “in-app purchases” events and did not record specific products of in-app purchases.
Therefore, the above in-app purchase tracking chart also plays a role as a
sample chart, and can change and add revenue as soon as specific information is available in reality. As can be seen, the highest number of purchases in the application is 2 times per day, and the lowest is 0 times per day. The average number of purchases in the app is 1.17 times/day.
From the sample charts above, the app publisher can update the chart if there is a change in the price of the ad, the form of the ad, and the products of the app. In addition, publishers can also devise strategies to increase ad revenue and increase revenue from in-app purchases, and use the chart above to track that increase. Furthermore, game publishers can also develop the above chart into an auto-updating chart, based on user data that is updated on a daily basis.
