### Covid Deaths Exploration 👋

<!--
**ngocanhp061/ngocanhp061** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
***Note:***
- Link of the code: https://github.com/ngocanhp061/ProjectPortfolio/blob/main/Project%201%20-%20covid%20death.sql

- Link of the visualization: *https://public.tableau.com/app/profile/pham.ngoc.anh1751/viz/CovidDashboardPortfolioProject_16625348695530/Dashboard1?publish=yes

**Step 0: Collecting dataset**

How I collected the dataset?

I visited the link: https://ourworldindata.org/covid-deaths  and download the full CSV file with the data from 28/01/2020 up to now.

**Step 1: ETL the origin CSV file and import into MS SQL Server**

I divided the owid-covid-data  CSV file into 2 excel workbooks (CovidDeath) and (CovidVaccination) for further purpose.
      
      Option 1: Import CSV files - FAILED
      
Normally, I often import CSV file into SQL Server. However, some columns in this file cannot be converted to the target datatype of SQL Server (for example: the datatype in CSV file cannot be converted to nvarchar in SQL) , so that the process of importing the CSV file failed.
     
      Option 2: Import Microsoft Excel 5.0/95 Workbooks - FAILED
      
The second option was to import Microsoft Excel 5.0/95 Workbooks. My origin dataset consisted of more than 85,000 rows. However, after saving as a Microsoft Excel 5.0/95 Workbook, it only had more than 16,000 rows.
      
      Option 3: Import Microsoft Excel 97-2013 Workbooks - FAILED
      
This is the second popular option that I often use - just after the option of CSV files. This kind of workbook just allow limited rows (around 65,000 rows), and 85,000 rows were too much for it. I did decide to choose it, because I thought 65,000 rows were not too bad for my first analysis. However, some data lost during the importing way, therefore, it eventually turned out that this way could not be used.
      
      Option 4: Import Microsoft 2007-2010 Excel file - SUCCEEDED 
      
P/s 1: The whole above process took me up to 1 hour to import the file. In the process, I did try to download the Excel file below the tutorial I followed, but he used the Microsoft 2007-2010 Excel file whereas that didn't work for me. I came across the error like this:
![image](https://user-images.githubusercontent.com/111174822/209476045-f595cd34-9268-4546-866a-9cf086826d65.png)


Then I found the solution on stackoverflow and it worked for me. After installing AccessDatabaseEngine, I could import the Microsoft 2007-2010 Excel file easily into SQL Server.

**Step 2: Explore data in SQL**

I did several steps to get some results in SQL, in order to visualize them on Tableau. You can find my SQL code via this Github link: https://github.com/ngocanhp061/ProjectPortfolio/blob/main/Project%201%20-%20covid%20death.sql

**Step 3: Visualize the data using Tableau**

I copied my SQL results into Excel (because Tableau doesn't have direct link with SQL). One thing I needed to notice in this step was: before visualizing on Tableau, I had to replace every "NULL" by "0" because "NULL" could cause errors in Tableau. Please feel free to visit my Tableau dashboard via: https://public.tableau.com/app/profile/pham.ngoc.anh1751/viz/CovidDashboardPortfolioProject_16625348695530/Dashboard1?publish=yes

**Step 4: My analysis**
****
![image](https://user-images.githubusercontent.com/111174822/209476235-9ca19fd2-ddb8-41f5-ae47-c9dc3ea9d7fd.png)

Until April 30th, 2021, there were 150,547,977 total infection cases, and 3,180,206 total deaths in the world. The amount of deaths accounted for 2.11% of the total cases.
Regarding the total deaths per continent, Europe ranked the first place with over 1 million deaths. North America and South America ranked the second and third place, with 847,942 and 672,415 deaths, respectively. Asia had 520,269 cases of death, just equalled one half of that in Europe, and ranked the fourth place, followed by Africa and Oceania. Africa recorded 121,784 total deaths, and the number in Oceania was about 1000 deaths.
About the Percent Population Infected line chart, I chose to show the five countries with the highest Population Infected Percentages, including the United States, Brazil, Russia, India and China. In August 2020, the population infected percentages in the US and Brazil started to faster than those in the 3 other countries (when Russia, India, China fluctuated around 0.1-0.6%, the percentages in US and Brazil were around 1.62%). The line of US and Brazil continued to go together until November 2020, when US's percentage started to be higher than Brazil and to rank the first place with 3.42%, followed by Brazil, Russia, India, China with 2.77%, 1.32%, 0.64%, 0.01%, respectively. The US recorded a rapid and continuous increase in the following months, reaching the highest increase of nearly 2% from December 2020 to January 2021, and finally reached 8.93% in March 2021. Brazil and Russia recorded a milder increase, and ended at 5.48% and 2.99% in March 2021, respectively. China recorded no increase, while India increased about 0.1% month-on-month.
I also used the Forecast tool of Tableau to estimate the percent population infected in the 5 countries mentiond above, and the US, Brazil, and Russia were predicted to have marked growth in the percentage of cases, while India and China were estimated to have very small growth.
The map chart reflected the percent population infected in each country. The countries with higher percentage were showed by darker color. It is easy to see that, the average percentage of population infected in US was highest with 9.77%, followed by some other South America countries such as Brazil, Argentina, and some Europe countries such as Sweden, France, etc.
