# JSON Data Based Exercise

Goals:
- Getting familiar with packages for dealing with JSON
- Study examples with JSON strings and files 
- Work on exercise to be completed and submitted 


Using Dataset: World Bank dataset from a school quality improvement project in Ethiopia. ('data/world_bank_projects.json')

1. Find the 10 countries with most projects
2. Find the top 10 major project themes (using column 'mjtheme_namecode')
3. In 2. above you will notice that some entries have only the code and the name is missing. Create a dataframe with the missing names filled in.

**Approach:**
1. Read the JSON into DataFrame
2. Sorting with groupby method to get project count and get top 10 countries
3. Read the JSON as a string to flatten the nested dictionary and normalize data
4. Get top 10 major project theme names by getting unique combination of code and name from original dataset
5. Redo top 10 major project themes including the mapped in theme names
6. Remove the duplicate associations of 'id' and project theme('mjtheme_namecode') code
7. Re-calculate top 10 major project themes and compare-contrast analysis
