# athletic_sales_analysis
*Objective*
The goal of this activity was to convert a set of athletic sales data into readable tables for the users. In order to accomplish this the program uses the three merging functions: **concat**, **grouby**, and **pivot_table**. 

*walkthrough* 
In order for the program to work some cleaning must be done first. The two csv files must be joined through the concat function in order to begin working on the data. After this is accomplished te program must check for null values and then datatypes of columns combined. Then the specific column must be changed to the datetime64 datatype if the later program operations will run smoothly. 

Once all of the groundwork has been laid then the program begins to get the information we are after. These tables will be crafted with both the groupby and pivot_table functions. They are designed to determine
    1. Which region sold the most sales
    2. Which region had the most products sold
    3. Which retailer had the most sales 

After these questions are answered then the program narrows its focus specifically onto "womens athletic footwear". From here the program repeats a similar process where both groupby and pivot_table are used to determine which retailer sold the most women's atheltic footwear. 

The last section of the program creates a pivot table with just "invoive date" and "Total sales". This table is designed to show total sales over a select period of time. In order to apply this kind of parameter to the program it needs to use a **resample** function. By doing this it can be determined
    1. The day with the most women's athletic footwear sales 
    2. The week with the most women's athletic footwear sales