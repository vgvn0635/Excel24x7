# How to Use Excel DATE Function?



![Excel Date Function](https://excel24x7.com/wp-content/uploads/Excel-Date-Function.webp)Excel Date Function


Date Function: A Brief



The Excel **DATE** function helps create a valid date using separate values for the **year**, **month**, and **day**. This function is useful when you need dates that update automatically based on other values in your worksheet.





ObjectiveValue Returned by functionAim to display or create date with **Year**, **Month** &amp; **Day**Date Function will return a **valid Excel date** in multiple forms. 



Date Function: A Syntax



`=DATE(year,month,day)`




- **Year**&#8211; Years mentioned in as Numbers.



- **Month**&#8211; Months mentioned in as Numbers.



- **Day**&#8211; Days mentioned in as Numbers.




Using Date Function with Practical Examples:



The **DATE** function in Excel creates a date using separate numbers for the year, month, and day. It returns a serial number that represents a valid date in Excel. To see the output as a proper date, apply a date format.





Using the **DATE** function is the most reliable way to create dates in Excel formulas. Unlike text-based dates, which can be misinterpreted, this function ensures that the year, month, and day values are clear and accurate.





Example 1: Hand Typed Dates as Numbers:



This is the basic and most common method to use the date function to display the proper excel date in the target cell based in the user provided numeric inputs. Refer to the below examples:





=DATE(1992,12,22)  //Displays- 22 December 1992
=DATE(2012,4,14)   //Displays- 14 April 2012
=DATE(2018,5,19)   //Displays- 19 May 2018

Choose the target cell, type the above syntax and hit Enter button to display results.



![Date Function Example displaying dates from hand typed numeric input data](https://excel24x7.com/wp-content/uploads/EXCEL_fAP1u4ppN7.webp)Date Function Example displaying dates from hand typed numeric input data


Example 2: Using Cell Reference to Execute Date Function:



The **DATE** function is helpful for creating dates that update automatically based on other values in a worksheet. For example, if **2023** is entered in cell **D1**, the formula below will return the date **July 20, 2023**:





**Note:** If **D1** is later changed to **2025** and the **DATE** function will update the result to show **July 20, 2025**.





=DATE(D16,7,20)  //Displays- 20 July 2023

Here- **D16** represents the value located in the cell D16.



![Date Function example using cell reference](https://excel24x7.com/wp-content/uploads/EXCEL_pkGb7NtKRW.webp)Date Function example using cell reference


![In Date Functions, output year value changes with cell reference value in real time](https://excel24x7.com/wp-content/uploads/EXCEL_PWnZ3k1XRs.gif)In Date Functions, output year value changes with cell reference value in real time


Example 3: Using DATE Function to display the First Day of the Present Year:



You can simply use the date function to display the first day of the present or current year and the formula to do this is, 





`=DATE(YEAR([TODAY](https://excel24x7.com/excel-functions/today-function/)()),1,1) // Displays- present year date (01 January 2025)`



![The simple formula display the first day of the present year using date function.](https://excel24x7.com/wp-content/uploads/EXCEL_1bereEa2yV.webp)The simple formula display the first day of the present year using date function.


Here to achieve this, I have used two more functions and they are: Year and Today functions. 






- **Year Function**&#8211; Displays the **year section** in the date with **4 digits**. 



- **Today Function**&#8211; Display the today&#8217;s date or current day date in the cell. 




This is an live example of **nesting multiple functions** in Excel. The **TODAY** function gets the **current date** and passes it to the **YEAR** function. The **YEAR** function **extracts the year** and sends it to the **DATE** function as the year value. The month and day are set to **1**, so the result is the first day of the current year, such as **&#8220;January 1, 2025&#8221;**.





Example 4: Combining with multiple complex functions such as Date Functions with SUMIFS, COUNTIFS:



You have a dataset containing sales records, where: **Column A** contains **sales dates**, **Column B** contains **sales amounts**, **Column C** contains **salesperson names**. If you want to find the following: Count the number of sales transactions after a specific date (e.g., January 1, 2023), Sum the total sales after that same date, Apply both conditions dynamically based on the year, month, and day values stored in separate cells.





**Formula to Count Sales After February 1, 2024**:





`=COUNTIF(A16:A21, "&gt;" &amp; DATE(2024,2,1))`



**Formula to Sum Sales After February 1, 2024**:





`=SUMIFS(B16:B21, A16:A21, "&gt;" &amp; DATE(2024,2,1))`



![Practical Example of using Date function with COUNTIF and SUM function in excel.](https://excel24x7.com/wp-content/uploads/EXCEL_LkyDTAVq5S.webp)Practical Example of using Date function with COUNTIF and SUM function in excel.


Verifying Answers from the above example manually: Count Explanation, Dates after February 1, 2024:






- 10-Feb-24



- 15-Mar-24



- 20-Mar-24



- 25-Apr-24




 Total count = **4**, Which is correct one. 





The SUMIFS result from the above formula (2600) is also correct because the sum of sales after Feb 1, 2024 is:






- 700 (Feb 10)



- 900 (Mar 15)



- 400 (Mar 20)



- 600 (Apr 25)




Adding all the value to get **2600** which is absolutely correct. Hence the above formula is proved correctly. In this way, you can use the Date function to make work with other complex functions to solve day to day needs. 






Interesting Tips about Date Function:






- The DATE function only accepts numeric values. If you enter text, it will return a **#VALUE!** error.



- The DATE function returns a **serial number** that represents a **valid date in Excel**.



- Excel dates start from the year **1990**. If you enter a year between **0 and 1990**, Excel will add **1990** to it.





That&#8217;s it.





&#8211; [Vigneshwaran Vijayakumar](https://excel24x7.com/creator/vigneshwaran/). 





Feel free to comment us below, if you have any queries about the above topic and find more interesting excel tutorials on our [homepage](https://excel24x7.com/). 





References: 




- **Date Function** by [CFI Team](https://corporatefinanceinstitute.com/), Retrieved on 08/03/2025: [Link](https://corporatefinanceinstitute.com/resources/excel/date-function-in-excel/) 



- **How to use the Excel DATE function** by [Chris Menard](https://www.youtube.com/@ChrisMenardTraining), Retrieved on 08/03/2025: [Link](https://www.youtube.com/watch?v=3OsamX6wG9s)



- **Date Function** by [Microsoft Support Team](https://support.microsoft.com/), Retrieved on 08/03/2025: [Link](https://support.microsoft.com/en-us/office/date-function-e36c0c8c-4104-49da-ab83-82328b832349)



- **Date Functions and Formulas in Excel** by [Technology for Teachers and Students](https://www.youtube.com/@techteachersandstudents), Retrieved on 08/03/25: [Link](https://www.youtube.com/watch?v=vXj0J5MgPTs)



- **How to Use Date Formulas in Excel** by [Custom Guide Team](https://www.customguide.com/), Retrieved on 08/03/2025: [Link](https://www.customguide.com/excel/excel-date-functions)