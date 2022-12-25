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

*  Link of the code: https://console.cloud.google.com/bigquery?sq=127863163697:05f09145051745b29801bd809a61f8e5

*  Link of the visualization: https://datastudio.google.com/reporting/3381df0e-ae57-4efd-9305-2a6094642e41/page/UrP4C

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


 👋 **Phân tích tình hình sử dụng app Flood it! (bản Tiếng Việt)**
 
 Flood it! là tựa game chiến thuật đơn giản, nơi mà nhiệm vụ của bạn là làm ngập màn hình bằng một màu duy nhất trong khoảng thời gian giới hạn. Bài phân tích này dựa trên dataset về dữ liệu người chơi của app này trong khoảng thời gian từ 12/06/2018 đến 03/10/2018. Bài phân tích sẽ trả lời được các câu hỏi chính sau đây:
 
- Số lượng người chơi dùng app mỗi ngày
- Số giờ trung bình mỗi ngày mà mỗi người chơi dùng
- Số giờ trung bình mỗi ngày mà mỗi người chơi dùng tại từng quốc gia
- Số lượng người chơi dùng mỗi hệ điều hành iOS và Android
- Tỉ lệ người dùng quay lại dùng app
- Số session trung bình mỗi ngày (session được định nghĩa là khoảng thời gian người dùng dùng app mà trong đó, thời gian không hoạt động nhỏ hơn 30 phút)
- Mẫu báo cáo theo dõi doanh thu từ app

**1. Số lượng người chơi dùng app mỗi ngày**
![image](https://user-images.githubusercontent.com/111174822/209474785-e557430d-fd52-462e-95c8-b9ec81ef72d7.png)


Biểu đồ trên thể hiện số lượng người chơi dùng app mỗi ngày trong khoảng thời gian từ 12/06/2018 - 03/10/2018. Có thể thấy, vào các ngày 18/6, 25/6, 28/6, 1/7, số lượng người chơi có xu hướng cao hơn hẳn các ngày còn lại, thậm chí là cao hơn gấp 3 lần so với bình thường. Đáng nói, các ngày trên đều là ngày thường và không phải cuối tuần. Tôi đã tìm hiểu về game này, nhưng game này có rất ít thông tin trên Internet. Có thể giả định là vào các ngày trên, game có sự kiện để thu hút người chơi nhiều hơn.
Trên thực tế, tôi cũng đã thử giả định rằng trong khoảng thời gian đó, game đổ bộ vào một thị trường mới nên thu hút thêm nhiều người chơi mới. Tuy nhiên, tôi đã quan sát biểu đồ thể hiện tổng số người chơi ở từng quốc gia ở bên dưới và nhận thấy:
![image](https://user-images.githubusercontent.com/111174822/209474796-f137f2fe-fa7c-468d-9dc9-1e1968749000.png)


Trong tất cả các ngày, Bắc Mỹ là khu vực có đông người chơi nhất. Kể cả vào các ngày 18/6, 25/6, 28/6, 1/7 nói trên, Bắc Mỹ vẫn là nơi có lượng người chơi đông nhất, và không có nơi nào có lượng người chơi tăng lên đáng kể trong các ngày này. Vì thế, giả định rằng game đổ bộ vào một thị trường mới trong các ngày này dẫn đến số người chơi tăng lên, là không khả thi trong trường hợp này.
Ngoài những ngày kể trên, các ngày còn lại đều có số lượng người chơi nhất định (dao động từ 400-500 người), chứng tỏ lượng người chơi của app này là rất ổn định.

**2. Số giờ trung bình mỗi ngày mà mỗi người chơi dùng**

![image](https://user-images.githubusercontent.com/111174822/209474806-8eea9145-bd16-4c4d-a35b-88fc75be2cfb.png)
![image](https://user-images.githubusercontent.com/111174822/209474816-cf0f6388-12c6-40ff-acc9-71f7ea6be62b.png)




Biểu đồ tiếp theo thể hiện số giờ trung bình theo từng ngày mà người chơi sử dụng để chơi game. Có thể thấy, số giờ trung bình dao động từ 2 giờ đến 4 giờ, với ngày có số giờ trung bình cao nhất là ngày 18/9, và ngày có số giờ trung bình thấp nhất là ngày 6/8.
![image](https://user-images.githubusercontent.com/111174822/209474837-db91934c-3d23-48c3-af5f-e1412df4069a.png)


Tính trong khoảng thời gian 4 tháng kể trên, số giờ trung bình mà người chơi sử dụng để chơi game mỗi ngày là 2.76 giờ.
**3. Số giờ trung bình mỗi ngày mà mỗi người chơi dùng tại từng quốc gia**
![image](https://user-images.githubusercontent.com/111174822/209474846-e2b412a1-8460-40bb-92f8-48937e16c2d6.png)



Biểu đồ bong bóng này thể hiện số giờ trung bình sử dụng app tại các quốc gia trên thế giới, với bong bóng càng to thì số giờ sử dụng trung bình càng cao. Có thể thấy bong bóng to nhất là ở nước Turkmenistan với trung bình người dân dùng đến 11 giờ mỗi ngày để chơi game. Dữ liệu này có thể cho thấy game đang được yêu thích ở các nước nào, để duy trì chiến lược kinh doanh ở các nước đó. Và với các nước mà game chưa được sử dụng nhiều, có thể mở rộng quảng cáo để thu hút người dân tại các quốc gia đó.

**4. Số lượng người chơi dùng mỗi hệ điều hành iOS và Android**

![image](https://user-images.githubusercontent.com/111174822/209474852-4e2a2c8b-02fe-4645-afc0-7b48f37f9f72.png)


Số người sử dụng của từng hệ điều hành được thống kê trong biểu đồ cột bên trên, với số lượng người dùng hệ điều hành iOS và Android là gần như ngang bằng nhau. Ngoài ra, có đến 1/8 số người là không xác định được hệ điều hành.

**5. Tỉ lệ người dùng quay lại dùng app**
![image](https://user-images.githubusercontent.com/111174822/209474860-64c2985e-18f8-4073-b0c4-412bbfe6d047.png)
![image](https://user-images.githubusercontent.com/111174822/209474865-3acb6626-b59e-4a10-8450-a0aa8909322f.png)





Tiếp theo là biểu đồ nhiệt dùng để phân tích tổ hợp (Cohort Analysis).  Trên thực tế, thành công lâu dài của những nhà phát triển ứng dụng không chỉ nằm ở số người download app , mà còn nằm ở việc duy trì lượng khách hàng quay trở lại vào app. Cohort analysis là công cụ rất hữu ích trong việc tính toán lượng người dùng dùng app qua thời gian.
Biểu đồ trên thể hiện phần trăm người dùng app qua thời gian, với màu đậm hơn là những ngày có tỉ lệ phần trăm cao hơn. Có thể thấy app duy trì được một lượng người dùng quay lại đều đặn. Trong tháng 6, tỉ lệ người dùng quay lại mỗi ngày là khoảng 4-7%, nhưng từ tháng 7 trở đi, tỉ lệ này giảm xuống thấp hơn, chỉ còn khoảng 2-4%. Đáng chú ý, tỉ lệ người dùng quay lại vào ngày 18/6 là cao nhất trong 4 tháng được xét.

**6. Số session trung bình mỗi ngày**
![image](https://user-images.githubusercontent.com/111174822/209474871-b4b86a0e-233e-4593-9699-3fbf51d3ae69.png)
![image](https://user-images.githubusercontent.com/111174822/209474873-f85f0b4d-af87-4e50-a4e8-7ba382c5e52b.png)




Sessions được định nghĩa là khoảng thời gian người dùng hoạt động trên app. Theo mặc định, nếu người dùng không hoạt động trong vòng 30 phút trở lên, thì hoạt động sau đó sẽ được tính vào session mới. Nói cách khác, trong mỗi session, khoảng thời gian mà người dùng không hoạt động phải nhỏ hơn 30 phút.
Biểu đồ trên thống kê số session trung bình mỗi ngày tại app Flood it! Trung bình một ngày có 106 session trên app.  Từ cuối tháng 6 đến hết kỳ, số session mỗi ngày dao động trong khoảng 75-150 session. Mặt khác, những ngày ghi nhận số người dùng tăng mạnh (như ngày 18/6, 25/6 và 28/6) thì có số session thấp hơn mức trung bình, với chỉ khoảng 50 session/1 ngày. Trên thực tế, số session trung bình mỗi ngày được tính bằng công thức:
![image](https://user-images.githubusercontent.com/111174822/209474876-4261f643-a4ef-4c92-9eb4-55b50d9ef643.png)
![image](https://user-images.githubusercontent.com/111174822/209474879-9df5ea33-f014-451c-a26e-a76fd0da79a3.png)




Tổng số người dùng và tổng số session mỗi ngày cũng được thống kê trong bảng trên. Có thể thấy, tổng số session mỗi ngày là gần như nhau, với khoảng 49,000 session. Tuy vậy, những ngày như ngày 18/6 có số lượng người dùng cao hơn hẳn, dẫn đến số session trung bình trong ngày giảm xuống thấp hơn mức trung bình.

**7. Mẫu báo cáo theo dõi doanh thu từ app**
Customer Lifetime Value (CLV) được định nghĩa là doanh thu được tạo ra từ người dùng trong khoảng thời gian người đó tương tác với app. Với Flood it! hay các game miễn phí khác, doanh thu này đến từ hai nguồn chính, bao gồm doanh thu từ quảng cáo và doanh thu từ mua hàng trên ứng dụng, trong đó quảng cáo đem đến doanh thu cao hơn. Vậy, câu hỏi dành cho các nhà phát triển ứng dụng là: làm thế nào để theo dõi lượng thay đổi doanh thu từ các nguồn trên?
Vì thế, trong bài phân tích này, tôi mang đến giải pháp cho bài toán này bằng mẫu báo cáo dưới đây.
![image](https://user-images.githubusercontent.com/111174822/209474884-b5b146dc-d0be-4895-a385-53fcf47ff4b2.png)


Biểu đồ này mang đến giải pháp để theo dõi số lượt chiếu quảng cáo và doanh thu từ quảng cáo qua các ngày. Quảng cáo cao đáng kể vào các ngày như 18/6, 24/6, 28/6, 16/9 (với khoảng 50 lượt quảng cáo). Đây cũng là những ngày ghi nhận lượng người dùng cao hơn so với các ngày khác. Từ đó, doanh thu thu được từ quảng cáo cũng cao đáng kể trong những ngày này. Ngoài ra, trung bình số quảng cáo đã được hiển thị mỗi ngày trong khoảng thời gian từ 12/6 đến 3/10 là khoảng 17 quảng cáo/ ngày.
Hai loại chi phí chính cho quảng cáo trên app và giá của từng loại tại thị trường Việt Nam bao gồm:
+ CPC (Cost per click: giá cho 1 lần bấm vào quảng cáo): 0.03 USD/click
+ CPM (Cost per 1000 impressions: giá cho 1000 lần hiển thị quảng cáo): 2USD/1000 lượt hiển thị, hay 0.002USD/1 lượt hiển thị.
Doanh thu trong biểu đồ trên được tính bằng công thức: 0.002 USD * số lượt hiển thị. Dữ liệu của app Flood it! được sử dụng trong bài phân tích này chỉ là dữ liệu mẫu, nên không ghi nhận quảng cáo được click, mà chỉ ghi nhận quảng cáo được hiển thị. Vì thế, biểu đồ trên đóng vai trò làm biểu đồ mẫu, có thể áp dụng tương tự cho các loại quảng cáo khác.
![image](https://user-images.githubusercontent.com/111174822/209474892-8b09d65a-a4a2-4f4f-a354-03d1aa5e7963.png)


Có thể có nhiều sản phẩm mua hàng trên ứng dụng khác nhau, ví dụ như:
+ mua gói VIP để trải nghiệm những dịch vụ hạn chế người dùng
+ mua gói không hiển thị quảng cáo
Giá của mỗi sản phẩm trên là khác nhau. Tôi cũng dùng biểu đồ tương tự như trên để thể hiện số lượt mua hàng trên ứng dụng trong khoảng thời gian được xét. Tuy nhiên, biểu đồ này không thể hiện doanh thu cụ thể, vì trong dữ liệu mẫu chỉ ghi nhận các lượt mua hàng trên ứng dụng, chứ không ghi nhận cụ thể là mua sản phẩm nào.  Vì thế, biểu đồ theo dõi lượt mua hàng trên cũng đóng vai trò là biểu đồ mẫu, và có thể thay đổi cũng như bổ sung thêm doanh thu ngay khi có thông tin cụ thể trong thực tế. Có thể thấy, lượt mua hàng trên ứng dụng cao nhất là 2 lượt, và thấp nhất là 0 lượt. Trung bình số lượt mua hàng trên ứng dụng là 1.17 lượt/ ngày.
Từ các biểu đồ mẫu trên, nhà phát hành app có thể cập nhật biểu đồ nếu có thay đổi từ giá của quảng cáo, hình thức của quảng cáo, và các sản phẩm tương ứng của app. Ngoài ra, các nhà phát hành cũng có thể đưa ra các chiến lược để tăng doanh thu từ quảng cáo và tăng doanh thu từ mua hàng trên ứng dụng, và sử dụng biểu đồ trên để theo dõi lượng tăng đó. Hơn thế nữa, nhà phát hành game cũng có thể phát triển biểu đồ trên thành biểu đồ tự động cập nhật, dựa vào dữ liệu người dùng được cập nhật hàng ngày.


