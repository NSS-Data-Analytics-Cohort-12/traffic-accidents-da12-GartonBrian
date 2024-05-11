# Nashville Traffic Accidents


For this exercise, you have been provided a dataset of traffic accidents that occurred in Davidson County which was retrieved from https://data.nashville.gov/Police/Traffic-Accidents/6v6w-hpcw. 

This spreadsheet has been divided into the following sheets:
* Accidents: Contains the raw data for each accident. In order to familiarize yourself with what is contained in each column, take some time to review the data dictionary here: https://data.nashville.gov/api/views/6v6w-hpcw/files/3af9281b-fa4f-4044-83f8-1b9a46cc6e95?download=true&filename=Traffic-Accidents-Metadata-v2.pdf.
* Analysis: This sheet will hold most of your answers.
* Zero Car Crashes: This sheet will be used in question 3.
* Collision Types: Contains the text description of each collision type. You will fill in your answers for question 5 here.
* Weather Types, Illumination Types, and Harmful Types: Contain descriptions for the other three codes. Not used in this exercise.


Use formulas to answer each question. Unless otherwise stated, fill in your answers in the "Analysis" tab.

1. How many total accidents are contained in this dataset? 
done

2. What are the earliest and latest records that appear in this dataset?
done

3. a. Create a new column to the right of the "Number of Motor Vehicles" column called "Single or Multiple". This column should contain "Single" if the number of vehicles is 1 and "Multiple" if it involved more than one vehicle. 
Used IFS instead of IF test for black cell and no cars involved otherwise as requested 
done

b. Are there any rows that involved zero vehicles? How many? Make sure that your formula accounts for these cases.  
done

c. Investigate the rows that have zero vehicles using the FILTER function in the "Zero Car Crashes" sheet. What do you find?  
That my table doesn't have headers and that irks me. I'm adding headers. I notice nothing. This needs a data visualization to matter to me
done

d. What percentage of crashes are single-car?
done

4. How many accidents occurred which are hit and run and had at least one injury?
done

5. a. What is the overall average number of injuries?  
done

b. Go to the "Collision Types" sheet and fill in the table to find the total number of crashes, average number of injuries, and total number of injuries per collision type. For each calculation, write a single formula and copy it down the table. What do you find? (Hint: If you're not sure how to answer this question, revisit the "Conditional functions and lookups" chapter of [Data Analysis in Spreadsheets](https://app.datacamp.com/learn/courses/data-analysis-in-spreadsheets).)
done

6. Add four new columns, Month, Year, Hour, and Weekday to the right of the Date and Time column. Use the [TEXT function](https://support.microsoft.com/en-us/office/text-function-20d5ac4d-7b94-49fd-bb38-93d29371225c) to extract out the Month, Year, Hour, and Weekday from the "Date and Time" column.  
done

7. Fill in the Hour table in the Analysis spreadsheet to find the number of accidents that occurred for each hour of the day. Again, write a single formula and copy it down the table. Do you see anything unusual? What might be the explanation for this?
done, the hours of the day with the most amount of cars on the road, rush hour, has the most amount of accidents followed closely by just after midnight. Should this not be caused by an error in our code one might assume that that is when the bars let out or that only the day and not time was entered by the original data imputer.
Done

8. Do the same for the year and day of the week. What stands out?
Done, 
Year: a 34k average amount of accidents occur with slight up cline, this may be proportional to the increase in population to the city And then COVID happened and a smaller amount of people drove though not as close to 0 as one might think with the majority of people sheltering.
Day: Again average number of cars on the road affect this alot, then I would assume dangerous activities would increase this, see above "when bars let out" comment. Would assume analyzation between, hours, area of town and other data could confirm or illuminate on this more

9. Add a column to the right of the Collision Type Code called "Collision Type". Use the table contained in the Collision Types sheet to fill in this column. 
We've got alot of tabs here please specify in every request where you want these columns to appear.
done

10. Which interstate has the most accidents between I-24, I-40, I-65, and I-440? Answer this by counting the number of accidents that contain the strings "I 24", "I 40", "I 65", or "I 440" in their Street Address. Hint: You may need to make use of [wildcards](https://support.microsoft.com/en-us/office/using-wildcard-characters-in-searches-ef94362e-9999-4350-ad74-4d2371110adb) in combination with the CONCAT function to answer this. Then do the same but search for "I24", "I40", "I65", and "I440" and then "I-24", "I-40", "I-65", and "I-440". Sum the results to get a total count. 


Consideration: there are different methods of describing the same roads EG: Highway 40, Interstate 40, HWY 40, that do not appear in the request. Recommend to user caution when interpreting the analysis 
Done


