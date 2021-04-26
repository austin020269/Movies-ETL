# Movies-ETL
UT Bootcamp Module 8 Challenge
## Project Overview
Movies and ratings data were acquired from both Wikipedia and Kaggle in order for students to use in a hackathon. We were asked to combine the data and save them into a SQL database for use in the event. To do this, we followed the ETL process data management rules which include: 

1. extracting the Wikipedia and Kaggle data 
2. transforming the datasets by cleaning them up and joining them together
3. loading the cleaned dataset into a SQL database

## Resources
Data Sources provided to analyze and minipulate included:
- ratings.csv
- movies_metadata.csv

Software utilized for this study included: 
- Python 3.7.6 
- Conda 4.9.2 
- Jupyter Notebook 6.1.4
- pgAdmin 4.30
- Personal GitHub account

## Analysis and Workflow

Deliverable 1:
1. Create a function to read in the three files and give it a name
2. Read in the movies_metadata and ratings CSV files as Pandas DataFrames
3. Open the Wikipedia JSON file and use the json.load() function to convert the JSON data to raw data
4. ead in the raw Wikipedia movie data as a Pandas DataFrame
5. Return the three DataFrames from the code provided.
6. se the variables provided to create a path to the Wikipedia data, the Kaggle metadata, and the MovieLens rating data files.
7. Set the three variables in Step 6 equal to the function created above
8. Set the DataFrames from the return statement equal to the data file names created above.
9. Check that all three files are converted to a DataFrame.

![alt text](https://github.com/austin020269/Movies-ETL/blob/main/Deliverable_1_pic.PNG)

Deliverable 2:
1; Add the code from this module for the clean movie function that takes in the argument "movie".
2. Add the function you created in Deliverable 1 that reads in the three data files.
3. Remove the code that creates the wiki_movies_df DataFrame from the wiki_movies_raw file and write a list that filters out TV shows from the wiki_movies_raw file.
4. Write a list to iterate through the cleaned wiki movies list.
5. Read in the cleaned movies list from Step 4 as a DataFrame.
6. Write a try-except block that will catch errors while extracting the IMDb IDs with a regular expression string and dropping any imdb_id duplicates. 
7. Write a list to keep the columns that have non-null values from the DataFrame created in Step 5, then create a wiki_movies_df DataFrame from the list.
8. Create a variable that will hold all the non-null values from the "Box office" column.
9. Convert the box office data created above to string values using the lambda and join functions.
10. Write a regular expression to match the six elements of form_one of the box office data.
11. Write a regular expression to match the three elements of form_two of the box office data.
12. Add the parse_dollars() function.
13. Add the code that cleans the box office column in the wiki_movies_df DataFrame using the form_one and form_two lists created above.
14. Add code that cleans the budget column in the wiki_movies_df DataFrame.
15. Add code that cleans the release date column in the wiki_movies_df DataFrame.
16. Add code that cleans the running time column in the wiki_movies_df DataFrame.
17. Use the variables provided to create a path to the Wikipedia data, the Kaggle metadata, and the MovieLens rating data files.
18. Set the three variables in Step 17 equal to the function created in Deliverable 1.
19. Set the wiki_movies_df equal to the wiki_file variable.
20. Check that your wiki_movies_df DataFrame

![alt text](https://github.com/austin020269/Movies-ETL/blob/main/Deliverable_2_pic.PNG)

## Summary

Specifically, me wanted to answer the following questions for the school district to summarize our study.

1. How is the district summary affected when reading and math scores are dropped fpr 9th graders at Thomas High School?
The % Passing of both math and reading dropped with the average math score decreased by 0.1 points.

2. How is the school summary affected?
The overall math and reading scores decreased for Thomas High School.

3. How does removing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools?
Thomas High School moved from 2nd place overall with a passing % of ~92% down to last place with a passing % of ~68%.

4. By removing 9th grade scores the following are effected:

- Math and Reading Scores by Grade - Thomas High School's 9th grade class has no math or reading score data to count. Everything else was unaffected.

- Scores by School Spending - The $630-644 bin saw a decrease in the passing percentages since Thomas High School was in that spending range. Though, interestingly the average math and reading scores for that range remained the same.

- Scores by School Size - The Medium (1000-2000) bin saw a decrease in the passing percentages since Thomas High School was in that school size. Though, interestingly the average math and reading scores for that range remained the same.

- Scores by School Type - The Charter schools saw a decrease in the passing percentages since Thomas High School was in that school type. Though, interestingly the average math and reading scores for that range remained the same.
