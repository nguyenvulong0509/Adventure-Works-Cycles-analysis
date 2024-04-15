# Adventure-Works-Cycles-analysis

### Introduction
_Adventure Works Cycles, a large, multinational manufacturing company, produces and distributes metal and composite bicycles to North American, European, and Asian commercial markets. While its base operation is located in Bothell, Washington, and employs 500 people, several regional sales teams are located throughout the company’s market region. In 2000, Adventure Works Cycles bought a small manufacturing plant, Wide World Importers, which is located in Mexico City, Mexico. Wide World Importers manufactures several critical subcomponents for the  Adventure Works Cycles product line. These subcomponents are shipped to the Bothell location for final product assembly. In 2001, Wide World Importers became the sole manufacturer and distributor of the touring bicycle product group. After a successful fiscal year, Adventure Works Cycles is looking to broaden its  market share by focusing its sales efforts on the company’s best customers, and reducing the cost  of sales by reducing production costs._

### About the project
- Sales representatives from regional sales offices have assigned sales territories in the United States, Canada, England, Australia, Germany, and France. Each regional office consists of several sales representatives and a team manager. In their daily sales activities, sales representatives use both laptops and Handheld PCs that run Microsoft® Windows CE. A typical work day for a sales representative starts with the representative dialing in to the regional office and downloading current data such as inventory, product, and promotional information. During customer visits, the sales representative takes orders on the laptop or Handheld PC. At the end of each day, the sales representative sets up appointments for the following day or week, checks the appointments of other representatives in the area for possible collaboration, and updates the contact list. The sales representative dials back into the regional office, sends updated information, and receives any new internal communications from the base office or regional office.
- When analyzing the insights of Sales Performance, the manager will comprehend the trend of the performance of each region through time series analysis, and recognize the region as either the potential one or not. Then, they will be supported to make good decisions for business strategies.

### Dataset
The AdventureWorks2019 dataset is stored in a public Google BigQuery dataset. To access the dataset, follow these steps:
- Open "Power BI desktop" then click on "Get Data" > More...
- In the search bar, type "Google Bigquery" then click on "Connect" > OK
- Click on "sign in" to log in by using your email
- After signing in > "Connect" > choose "adventureworks2019" database to get access on desired tables

To know more about tables' fields, see the data dictionary in this repository

 ### Visualisation and insights

#### 1. Overall performance
 
![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/84d15645-3e23-4715-a530-bd8a68e4c12d)

- First of all, we can see that the company's business situation appears relatively good through indicators such as Total Orders, Total Sales, and AVG Sales per Product. However, the issue here was that the costs (Total Cost) were quite high (100.47/109.85m). This led to the consequence that despite having a high number of orders and sales, the profit was low (9.37m profit – approximately a 10% profit margin).

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/3c48a41c-5a43-41a3-b2b2-e47b27de5ab8)


- Furthermore, although there was overall growth in business performance from 2011 to 2014 (increasing by about 10m throughout the period), the figures are not significant. After 2013, there was a significant decline in revenue (43m > 23m).

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/b6aad087-fb5f-4dd7-8acf-0aedc8d139b1)

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/bc82ba53-1823-4e10-8b18-94e82e627884)

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/fac6d23d-a73f-4e6b-bd1e-af65b6ae990c)

- It can be seen that although North America leads in Total Sales (possibly because it has been selling all 4 product groups since 2011 while the other two regions started selling Accessories, Clothing, and Components after 2011), it has lower Profit compared to the other two regions. The reason could be that the Southeast, Northeast, and Central regions have negative profit (refer to the dashboard for more details). Additionally, the Pacific region, despite having the lowest Sales, leads in Profit with 3.43m.

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/a3586087-647e-4112-9437-56fb36de5517)

- It turned out that the Southwest region in the US has the highest Cost. This also contributes to explaining why the Profit of North America is lower than that of Europe and the Pacific.
- Finally, we will consider the products along with the information obtained from the analysis of the regions.

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/7a303b3a-7b59-40c3-a0b2-6e5078fc3ccd)

- In general, Bikes have the highest number of Orders, while Components have the lowest. However, despite having a high number of Orders (35000), the Sales of Accessories are relatively low (approximately close to 800k - possibly due to the lower AVG price of this product group compared to others). Nevertheless, the Profit of Accessories is higher (420K) compared to the two product groups, Clothing (-65K) and Components (90K).
- Digging deeper into the Clothing group, most countries have negative profits except for Northwest – US and Australia.
- The Components group provides relatively stable profits for most countries except for Germany and Australia, with only about 3-5k Profit.
- Further into Accessories, it can be seen that the Road Bottle Cage product has quite low Orders and Sales.

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/1c156922-a282-4752-ab4e-4bef37b6bbd8)

- For Clothing, Sales mainly come from Jerseys, while the issue lies with Gloves and full finger gloves.

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/320d4a91-a58e-4796-b75d-eb35f6debf3b)

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/522c892d-ad7a-4718-adbf-d071c0aa33ae)


#### 2. Sale performance

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/f1928362-1122-4598-aa96-a57122ad998e)

- Overall, the company's online sales are relatively developed (60k/121k orders), and the AVG Sales per Order is quite good. However, Total online sales are relatively low (29.6/109M) despite online orders accounting for 50% of the total orders of the company. Additionally, the number of items per order is also low (on average, only 1 product is purchased per order).

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/f6ca8977-d416-42ea-8dd9-61ef060362f2)

- The North America region continues to lead in online sales. However, when looking at the map and charts, it can be observed that the three regions Southeast, Northeast, and Central are less developed in online sales (the Online to Total Sales ratio of these regions is relatively low), leading to negative profits and low profits as analyzed in the overall performance.

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/d5393097-c104-458e-b06f-dc6c413749f0)

- However, when considering individual countries, Australia leads in Online to Total Sales ratio. Meanwhile, Canada and regions of the US have lower ratios (with only Southwest – US, Northwest – US, and Canada maintaining the ratio at a moderate level).

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/ef219c0c-9b81-42f2-aab1-60c33aac0f2e)

- This could also be similarly described with Successful Orders and Successful Sales.

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/34df73ab-b645-42f7-b7a5-ed3e683302cb)

- Based on the chart, it can be seen that Online Orders of Accessories are the highest, but the AVG Sales per Order is significantly lower compared to Bikes. The reason could be that the price of each product in the Accessories group is lower than that of Bikes (36 < 1200). Additionally, the Components group has no Online Orders. The Clothing group has relatively low Orders and brings in fewer Sales compared to the other two groups.

- Digging deeper into Sub-categories, Clothing – Socks should be noted as both the number of Orders and AVG Sales per Order are relatively low at the same time.

![image](https://github.com/nguyenvulong0509/Adventure-Works-Cycles-analysis/assets/116187817/1cfb9eb1-97ba-465c-bb22-511bfb09e8d9)

### Recommendations
- The company needs to find ways to reduce overall costs to maximize profits. This includes reducing costs for the Southwest region, as it accounts for a quarter of the expenses.
- The Pacific market shows relatively large potential for development due to its high profits, despite having only one country (similar to online).
- There is a need to focus on improving business performance in the Southeast, Northeast, and Central regions (similar to online).
- Consideration can be given to increasing prices for the Accessories product group.
- Efforts should be made to understand and improve the Clothing product group to increase sales and revenue (similar to online).
- Further investigation is needed into why there are many online orders but low sales.
- Strategies should be developed to increase the number of products per order (through promotions, quality improvements, presentation, etc.).
- Promoting the Components group on the online platform can help increase sales.






