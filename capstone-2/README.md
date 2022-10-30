## **Vehicle Fuel Economy \|** ![](images/excel.svg)

> ### **Business Analysis for Lariat Rent-A-Car**
>
> -   `Examined and cleaned historical sales data using Excel (VLookUp, pivot tables and t-tests)`
>
> -   `Facilitated exploratory data analysis and assessed by KPI performance.`
>
> -   `Developed and presented models that showcased a 40% increase in profits.`
>
> *Click the icons below to see the project files and deliverables*  
>
> | Excel | PowerPoint | ReadMe |
> | :-: | :-: | :-: |
> |[<img src="images/filetype-xlsx.svg" width="54px">](https://1drv.ms/x/s!Ahpkb3AfX4xfgsA0TbaqsDQorD8vKA?e=vEQXVr)|[<img src="images/filetype-pptx.svg" width="54px">](https://1drv.ms/p/s!Ahpkb3AfX4xfgsAztt7OBQG6rwSqYg?e=HYOXor)|[<img src="images/github.svg" width="45px">](https://github.com/bradfordjohnson/thinkful/tree/main/capstone-1)|
---
![](images/lariat.jpg)
## **❓ Business Objective** 
> ### *Lariat’s* **business objective**: `minimize their costs` and `maximize their revenue`  
> This was my **first Thinkful Capstone project**, and I was playing the role of a data analyst consultant for [*Lariat*](https://fictionalcompanies.fandom.com/wiki/Lariat_Rent-A-Car). *Lariat* is a fictious car rental company which has a fleet of **4,000 rental cars**, **72 different car makes** and **878 unique car models** ranging from the years 2016-2018.  
>
> *Lariat* also wanted me to **develop two deliverables** for them, the first being an **Excel model** which contains dynamic and static charts, and a model which allows users to manipulate business parameters and see the results of those changes. The second deliverable was a **PowerPoint** which shows the data analysis process, and shares insights with *Lariat* executives. Finally, I **presented** my slides and model to a Thinkful official who was playing the role of a *Lariat* executive.
## **📊 The Data**
> *Lariat* provided me with 4 Excel Workbooks, each of the Workbooks contained **different** data:
> - Workbook 1 - **Fleet vehicle data:** `Car ID, Make, Model, Year...`
> - Workbook 2 - **Cost data:** `Car ID, Monthly cost, Insurance Costs...` 
> - Workbook 3 - **Transaction data:** `Car ID, Revenue, Branch ID, Dates...`
> - Workbook 4 - **Branch data:** `Branch ID, State, City, Airport?...`
> 
> The Workbooks and columns are set up like a **SQL database**, with relational data tables, and keys that connect the different tables. The structure of the data is important to understand as this will tell you what formulas can be used to combine the data, and how to **interpret** each “table”. 
> 
> After consolidating the Workbooks, I cleaned up the data and began to explore it with **pivot charts** and **tables**. I also began combining the data using formulas to make this data tell its story. 
> 
> The **most common** formulas I used include: `=VLOOKUP()`, `=XLOOKUP()`, `=SUMIF()`, and `=IF()`.

## **📐 Methods**
> The first thing I wanted to get from combining the data was the **revenue**, **costs**, and **profit** for all of the 4,000 fleet rental cars by the **month**, and then for the **year**.  
> 
> The data was **missing records** for December and most of November, so I had to do without, however with the cell references I used, this is not a problem as post analysis additional data can be added and the Workbook, all the formulas, and the model would update and be accurate. 
> Once I had built out my formulas, I explored my data further with `pivot tables` and `charts`.  This let me see trends in the **profitability of different car makes and models**. I explored potential trends such as by branch, however with the variability of the locations and markets it would need more data before any trend of significance is noticed. 
> > *For example comparing an airport branch that is in a medium sized city on the East Coast of the US to a non-airport branch on the West Coast in very dense metropolitan area would not be fair.* 
> 
> When it comes to the deliverables, the Excel model was designed to have a **baseline** for *Lariat*. This baseline would be broken down by the three rental `car model years`. The metrics would be the `daily revenue`, `costs`, and `number of rentals for the year`. This would show the current daily state of the business, and my model would be a user scenario for stakeholders to input their own values to see how changes in costs, revenue, or rental days impacts the yearly figures. This would be able to allow stakeholders to use the model to make informed business decisions.
>   
> > *Baseline Visual*
> > 
> > ![](images/baseline.png)
>
> <br>
> 
> > *User Scenario Visual*
> > 
> > ![](images/user.png)
> > As you can see in the *above* image, there are **data input fields** where users can input percentages and manipulate the percentage change from the baseline metrics. Such as **simulating a decrease in cost** or **increase in revenue** and **proportionate changes in the number of rentals**. 
> > 
> > **Included in the Excel Workbook** is *documentation* for the model and how it works. I also implemented **data validation** and **protection** to keep from unintended changes being made, and unintended inputs.
## **📈 Insights**
> *NOTE: These are only some of the insights, you can find more in the Excel Workbook*
> 
> There was **not a significant difference** in the number of rental days between the 3 different car model years. 
>
> ![](images/year-bar.png) 
>
> *Ford*, *Chevrolet*, *Dodge* and *Toyota* were the **top 4 car makes by revenue**. However, these 4 makes account for over **25%** of the fleet’s cars.
> 
> ![](images/revenue-bar.png)
>
> These are some cars *Lariat* needs to **get rid of**, as they are not profitable.
>
> ![](images/noprofit-table.png)
> 
> The difference in *Lariat's* actual profit and their user scenario profit. This scenario is the same user scenario as *above*, and this is the dynamic chart that changes with the **user's input** to the model.
>
> ![](images/profit-bar.png)
## **💬 Discussion**
> *Lariat's* **business objective** was to minimize costs and maximize profits. I suggested to *Lariat* ways to meet this objective, and here is my suggestion:
> - Minimize costs by converting fleet to the most profitable vehicles. Sell the vehicles that are not profitable.  
> - Maximize revenue by increasing the rental prices for fleet vehicles.
> - Assume a decrease in rental days.
>
> I decided for my Excel model to group the cars by model year, this is because older vehicles may need more servicing and repairs than newer cars. When I think of *new cars*, I think of the *new features* for the end user. This is also a good way to split up the fleet into groups of cars for the user scenario inputs.
