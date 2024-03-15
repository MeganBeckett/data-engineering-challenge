# data-engineering-challenge

**Challenge: Wrangle the raw data into a useable format and and design basic data infrastructure for a Global Health project**

### Context

As a Data Engineer on a Global Health Project, looking at vaccine supply and demand forecasting in the country Verdania, you are investigating setting up a data pipeline to pull data from the country's health data system, wrangle it and insert into your own database.

You have been given a sample data file from querying the API endpoint `regional_vaccine_supply` for the health data system which tracks vaccine supply to health facilities at the regional level. The data received is in `json` format and is nested.

To perform efficient analytics, you need to flatten the JSON structure into a tabular format. The goal is to create a flat table that can be easily loaded into a database and additionally, the Machine Learning team would like CSVs of the data to start the modelling process. There is also information about each vaccine that needs to be extracted into a separate CSV file.

### Challenge steps

The following is a guideline of the minimal steps to follow:

1. Flatten the JSON Structure:

Write a program or script to flatten the nested JSON structure into a flat table. Each row should represent a unique combination of region, vaccine type, date, and amount of supply.

2. Create a CSV for Vaccine Information:

Extract information about each vaccine from the "vaccine_information" section and save it as a separate CSV file named "vaccine_information.csv". Include columns for vaccine type, manufacturer, storage conditions, and doses required.

3. Design a Relational Database Model:

Design a relational database model to store the data. Use SQL to create the necessary tables and define relationships.

4. Handle Missing Values:

Handle cases where certain supply dates are not present for a particular region or vaccine type. Use appropriate placeholders (e.g., NULL or 0) for missing values.

5. Generate a CSV Output for Vaccine Supply:

Save the flattened supply data as a CSV file named "flattened_vaccine_supply.csv".

6. Documentation:

Provide a brief explanation of your code, including any assumptions or design choices made during the flattening process and database model design.

7. Bonus - Version control:

Submit your challenge using a version control system, such as Github, to demonstrate use of versioning.