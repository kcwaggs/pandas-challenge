# pandas-challenge
## Module 4 Challenge

# ANALYSIS
In this report we are analyzing 15 different high schools with different spending budgets, headcounts, scores and type of school. In total we are reviewing 39,170 students and honing in on their math and reading scores and pass rates. In order to see trends, we also compared the students' scores and pass rates to their class grade (9th-12th), per student budget, school size, and school type. In review of this information the main focus I want to identify is looking at the school TYPE as a differentiator. 

From the results I drew, it became clear early on that charter school and district school results were going to vary. In the the highest performing schools section, every school in the top 5 is a charter school; on the flip, every school in the bottom 5 are district schools. Something to note here, the 'Total Students' section in these tables show that the top schools were vastly smaller than the bottom schools with a 634 student headcount difference between the biggest school in the top 5 and the smallest school in the bottom 5. This also gets further visualized in the size_summary results where the large schools scores were much lower than both the small and medium schools. 

In terms of spend; the lowest spending range per student results out-performed every other spending range. Transversely, the largest spending range per student had the lowest results out of all the other spending ranges. If you revisit the school_spending_df table, you will see that every school in the '<$585' spending range is a charter school and every school in the '$645-$680 spending range is a district school. I think this paints a really clear picture about resources provided at different school types. Charter schools will almost always have better, newer, more advanced resourcing than district schools and therefore will not require additional budget to bridge the gap and improve test scores. This is further reiterated in the final type_summary table where charter schools outperformed district schools in every category. 

In summation - if further analysis were to be done on schools in this region/state, I would recommend grouping the results by school type and then conducting the analysis. I believe that having them together for this review skewed the data and does not give us actionable insight on how to improve test scores for the schools. However, if we group the schools by type (aka: by their alotted resources), we might find more valuable insight and determine if these factors can help play a part in score improvement. 

## Dependencies: 
Data pack link: https://static.bc-edx.com/data/dl-1-2/m4/lms/starter/Starter_Code.zip
I used the the starter file from the data pack to begin my analysis
    PyCitySchools_starter.ipynb
    Renamed to: PyCitySchools.ipynb

I found that with nearly every step you can calculate fields by using the separated CSV files or the merged files. I was attempting to track two different files with two different methodologies to solving the calculatios. I ended up leaning into using the merged CSV file as this is more similar to the kind of data I am working with at my job.

In terms of my results - I ended up formatting my results for % values rounded to one decimal place and averages rounded to 2 decimal places. I also removed the decimals in the total budget and per student budget because the results I was receiving did not retrieve any values for cents. 
The outliers to this formatting are the school_spending_df and size_summary initial prints after adding the pd.cut. as formatting was conducting after this step. 

## Resources:

Using .drop_duplicates: https://stackoverflow.com/questions/23667369/drop-all-duplicate-rows-across-multiple-columns-in-python-pandas
Formatting for % and decimal places: https://saturncloud.io/blog/how-to-format-certain-floating-dataframe-columns-into-percentage-in-pandas/#:~:text=To%20format%20the%20Discount%20column,each%20value%20in%20the%20column.
Rounding decimals: https://www.freecodecamp.org/news/how-to-round-a-float-in-pandas/#:~:text=Pandas%20round()%20Method%20Example&text=round(2)%20return%20rounds%20a%20number%20to%20two%20decimal%20places.
Change Index Column Name: https://sparkbyexamples.com/pandas/pandas-set-index-name-to-dataframe/
Converting currency back to float: https://stackoverflow.com/questions/32464280/how-to-convert-currency-column-with-and-to-numbers
