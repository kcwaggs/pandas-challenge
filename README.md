# pandas-challenge
## Module 4 Challenge

## Dependencies: 
Data pack link: https://static.bc-edx.com/data/dl-1-2/m4/lms/starter/Starter_Code.zip
I used the the starter file from the data pack to begin my analysis
    PyCitySchools_starter.ipynb
    Renamed to: PyCitySchools.ipynb

## Notes:
When I first calculated the total budget, I did not think to use the separate CSV files to calculate it. I ended up formulating the total based on the merged dataframe. After some review I realized I could have simplified this by calculating the total budget from the original 'schools_complete.csv'. I ended up creating 'total_budget' and 'total_budget_2' inputs to show you my calculations from 1 - the merged dataset 2 - reading the original CSV file. 

I found that with nearly every step you can calculate fields by using the separated CSV files or the merged files. I am attempting to do both methods to better understand the data manipulation. Most likely, in my work I would be using one large file as compared to merging two files. 
>>> I ended up creating a secondary .ipynb file to track these calculations in different files. 

## Resources:

Using .drop_duplicates: https://stackoverflow.com/questions/23667369/drop-all-duplicate-rows-across-multiple-columns-in-python-pandas
Formatting for % and decimal places: https://saturncloud.io/blog/how-to-format-certain-floating-dataframe-columns-into-percentage-in-pandas/#:~:text=To%20format%20the%20Discount%20column,each%20value%20in%20the%20column.
Rounding decimals: https://www.freecodecamp.org/news/how-to-round-a-float-in-pandas/#:~:text=Pandas%20round()%20Method%20Example&text=round(2)%20return%20rounds%20a%20number%20to%20two%20decimal%20places.
Change Index Column Name: https://sparkbyexamples.com/pandas/pandas-set-index-name-to-dataframe/
Converting currency back to float: https://stackoverflow.com/questions/32464280/how-to-convert-currency-column-with-and-to-numbers
