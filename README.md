## KPMG_Virtual_Intership_Data_cleaning
 Thank you for providing us with the three datasets from Sprocket Central Pty Ltd. The below table highlights the summary statistics from the three datasets received.
 
**Transaction table missing records**
*	online_order               360
*	brand                      197
*	product_line               197
*	product_class              197
*	product_size               197
*standard_cost              197
*	product_first_sold_date    197

**customer Demographics**
*	customer_id                              1
*	last_name                              125
* DOB                                     87
*	job_industry_category         656
*	default                                302
*	tenure                                  87

 Notable data quality issues that were encountered and the methods used to mitigate the identified data inconsistencies are as follows. Furthermore, recommendations have been provided to avoid the reoccurrence of data quality issues and improve the accuracy of the underlying data used to drive business decisions.
 
**Inconsistent values for the same attribute**

for instance in the Gender column for Customer demographics,  ( ['F', 'Male', 'Female', 'U', 'Femal', 'M'] instead of consistently applying 'Female', 'Male', 'U' to describe gender 

 **Recommendations:** 
 Enforce a drop-down list for the user entering the data rather than a free text field. In order to construct meaningful variables for the model, the data has been cleaned to avoid multiple representations of the same value. 
 
**Invalid values**
The DOB has values that appear invalid, e.g 1843-12-21 00:00:00.

**Recommendation:** add constraints on the minimum value that should be entered into this field.
