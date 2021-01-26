# Set up a New Budget

There are two custom records that you need to understand to be able to set up any kind of budget with Alterview BOA

![](RackMultipart20210126-4-ujurt4_html_56069d386a327c14.png) ![](RackMultipart20210126-4-ujurt4_html_20e58fa56cfbf8f8.gif) ![](RackMultipart20210126-4-ujurt4_html_20e58fa56cfbf8f8.gif)

**Alterview BOA Budget on Anything:** This record has two functions:

- Register Budget
- Define records to create budget on

**Alterview BOA Budget Type:** This record has one function: Define the budget types you like to use. There are several pre defined included, but you can create as many as you like.

**Set up a New Budget Type**
**Alterview BOA Budget on Anything:**

This record includes 5 list/records that gives you possibility to create budget based on: CLASS, DEPARTMENT, EMPLOYEE, CUSTOMER, ENTITY.

![](RackMultipart20210126-4-ujurt4_html_18c4362827e34800.png) ![](RackMultipart20210126-4-ujurt4_html_8e942a8118777027.gif)

If you like to create a Budget based on a record that is not defined above, for example a Custom Record, just click on New Field and add another field. The field should be of the type List/record and point on the record type you like to base your budget on. Follow the naming standard for the internal id: custrecord\_avns\_boa\_\&lt;customrecord\&gt;.

When the list/record that you like to base your budget on is defined above you go to the record Alterview BOA Budget Type.

![](RackMultipart20210126-4-ujurt4_html_a9a4c13a95488f58.png)

If the budget type you like to have is not defined you have to set it up.
 To define a new budget type click on &quot;New Alterview BOA Budget Type&quot;

![](RackMultipart20210126-4-ujurt4_html_36fb1d69f4274226.png)

**Name:** Budget Type a Name – In this example I call it Customer Sales Budget
**Field ID:** The field id should be any of the field id´s that is defined in the record Alterview BOA Budget on Anything.

![](RackMultipart20210126-4-ujurt4_html_e9dc8f54cbfa4800.gif) ![](RackMultipart20210126-4-ujurt4_html_18c4362827e34800.png)

The budget type Customer Sales Budget is a budget based on customer, therefor I fil in custrecord\_avns\_boa\_customer in the field ID in this example.

## Set up a new budget

Now you are ready to set up a budget. Go to Alterview BOA Budget on Anything and click on &quot;New Alterview BOA Budget on Anything&quot;
 ![](RackMultipart20210126-4-ujurt4_html_a44cb79df1376c8.png)

![](RackMultipart20210126-4-ujurt4_html_626f45ea3781efc8.png)

**Budget For:** Chose the budget type you like to use.
**Customer:** In this case the budget type is based on customer record and therefor the field customer is showing (if the budget type would have been based on a custom record or department or any other list/record, that list/record should have been send here instead). Chose the customer you like to set up a budget for.
**Period Type:** You can chose Day, Week, Month or Year. If you chose month, 12 budget rows will be created, if you chose week, 52 rows will be created (if start date is 1 of January and End Date is 31 of December).

**Start Date:** Chose start date. Usually 1 of January

**End Date:** Chose end date. Usually 31 of December, same year as start date

**Amount:** Chose the budget amount for the full period. Your amount will be even distributed among the created budget rows. You use this field if your budget is based on money (example sales by sales rep per month).

**Number:** Chose the budget number. Your number will be even distributed among the created budget rows. You use this field if your budget is based on numbers (example nr of phone calls made per month).

When you are done, click on Save
 ![](RackMultipart20210126-4-ujurt4_html_cd735d5698ac8b94.png)
 When the record is saved click on the update button.

![](RackMultipart20210126-4-ujurt4_html_f09365c9843ae7db.png)
 Now the Amont is distributed even amongs the budget rows. If you need you can go in and move the amount between the different months to better fit your budget plan.

# Follow up on your Budget

There are several ways to follow up on a budget. In this chapter we gone show you 2 ways to do it

##
 Budget tab

A logic place to find your budget is on the record you have created your budget for. In the above example it is on the customer record.

S ![](RackMultipart20210126-4-ujurt4_html_fe4ab55e4525a21c.gif) tep 1: Create a Saved Search: BOA Customer Sales Budget
 ![](RackMultipart20210126-4-ujurt4_html_40271b7e1133730a.png)

![](RackMultipart20210126-4-ujurt4_html_2c3c9626b75faa79.png) ![](RackMultipart20210126-4-ujurt4_html_d39cbfa061219a46.gif)

**Search Title** : Give the search a title (we suggest you follow naming standard BOA + budget type)
**Available as Sublist View** : Check this checkbox to be able to include on tab on customer record.

Criteria
**Filter:** Budget For: Chose your budget type

![](RackMultipart20210126-4-ujurt4_html_1edec041a6da5856.png)

Sort by: Start Date

Fields
 Start Date
 Amount (if the budget is based on money)
 Number (if budget is based on numbers)

![](RackMultipart20210126-4-ujurt4_html_3a5aa97de91aaefd.png)

Filter: Customer (if budget is based on customer you chose customer here)

Step 2: Create a Search for Actual Result

**Step 2: Set up a Budget Tabs**

![](RackMultipart20210126-4-ujurt4_html_c1f2dd2e263c8e97.png)
 Navigation: Customize  Forms  Subtabs

![](RackMultipart20210126-4-ujurt4_html_d71d8f0edafa6bcd.png)

Create a new Tab: Budgets

![](RackMultipart20210126-4-ujurt4_html_e71eb9a8aa5d2302.png)

Create a second tab: Sales Budget. Chose Budgets as Parent.

**Step 3: Set up a Sublist**
 ![](RackMultipart20210126-4-ujurt4_html_cd40d8656c52c4a0.png)

Navigation: Customize  Forms  Sublists

![](RackMultipart20210126-4-ujurt4_html_83067c0e1ab10fe8.png)

Search: chose your search
 Label: Set lable for subtabe
 Tab: Chose the tab you created

Customer: Check the entity where to show your budget, in this case Customer

Repeat this step for both searches.

**Step 4: See the Result**
 ![](RackMultipart20210126-4-ujurt4_html_bddcea302ed947b.png)
 Open the customer and control the result

If you like to compare your budget to an actual number, just add another search
 In this exemple we create a BOA Actual Sales Search
 ![](RackMultipart20210126-4-ujurt4_html_c0819a039285fdd4.png)

![](RackMultipart20210126-4-ujurt4_html_29f4971b5fea998e.png) ![](RackMultipart20210126-4-ujurt4_html_82100709a12d391a.png) ![](RackMultipart20210126-4-ujurt4_html_80e7b380162c57ff.png)
 Navigation: Customization  Forms  Sublists

![](RackMultipart20210126-4-ujurt4_html_4ea003ef090c4438.png)Add the new search.
