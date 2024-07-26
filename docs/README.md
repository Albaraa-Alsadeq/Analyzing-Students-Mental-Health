# Student Data Analysis Project Using PostgreSQL


![Description of the image](https://github.com/Albaraa-Alsadeq/Analyzing-Students-Mental-Health/blob/main/photo_1.png?raw=true)




## Project Description
Studying abroad can be both exciting and difficult. But what might be contributing to this? One Japanese international university decided to find out!

Use your data manipulation skills to explore the data from a study on the mental health of international students, and find out which factors may have the greatest impact.

Does going to university in a different country affect your mental health? A Japanese international university surveyed its students in 2018 and published a study the following year that was approved by several ethical and regulatory boards.

The study found that international students have a higher risk of mental health difficulties than the general population, and that social connectedness (belonging to a social group) and acculturative stress (stress associated with joining a new culture) are predictive of depression.

Explore the students data using PostgreSQL to find out if you would come to a similar conclusion for international students and see if the length of stay is a contributing factor.

Here is a data description of the columns you may find helpful.

Field Name    | Description
-----------------------------
inter_dom     |	Types of students (international or domestic)
japanese_cate |	Japanese language proficiency
english_cate  |	English language proficiency
academic      |	Current academic level (undergraduate or graduate)
age	      | Current age of student
stay	      | Current length of stay in years
todep	      | Total score of depression (PHQ-9 test)
tosc	      | Total score of social connectedness (SCS test)
toas	      | Total score of acculturative stress (ASISS test)



## How to Use
1. Create the database:
    ```sh
    psql -f scripts/create_database.sql
    ```
2. Create the tables:
    ```sh
    psql -d university_data -f scripts/create_tables.sql
    ```
3. Load data from the CSV file:
    ```sh
    psql -d university_data -f scripts/load_data.sql
    ```
4. Execute the analytical queries:
    ```sh
    psql -d university_data -f scripts/analysis.sql
    ```

## Files
- `data/students.csv`: Contains student data.
- `scripts/create_database.sql`: To create the database.
- `scripts/create_tables.sql`: To create the tables.
- `scripts/load_data.sql`: To import data from the CSV file.
- `scripts/analysis.sql`: Analytical queries.

## Requirements
- PostgreSQL
- psql
