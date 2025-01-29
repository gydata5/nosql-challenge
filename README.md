# NoSQL Challenge: Food Establishments Database

# Overview
The NoSQl Challenge project involves analyzing and updating a MongoDB database containing food establishments in the UK, while focusing on their food hygiene ratings. This project includes setting up a MongoDB database, importing and updating data, and performing exploratory analysis on the data using MongoDB queries and Python. The data is sourced from the UK Food Standards Agency and includes various fields related to food hygiene ratings, establishment information, and location details. 
# Project Details
* no_sql_challenge/: My root directory of the project.
* NoSQL_GYoung.ipynb: Notebook for setting up the database and importing data.
* NoSQL_analysis_GYoung.ipynb: Notebook for performing exploratory analysis on the database.
* Resources/: Folder containing the establishments.json file.
  * establishments.json: JSON file containing data of food establishments in the UK.
# Part 1: Database and Jupyter Notebook Set Up
  1. Create the MongoDB database:
     * Import data from establishments.json into a MongoDB database called **uk_food** with a collection called **establishments**.
     * Use **PyMongo and Pretty Print** libraries to interact with MongoDB and display data.
  2. Confirm the database uk_food is created.
     * List the collections to ensure establishments is loaded correctly.
     * Query a single document using **find_one()** and display it using pprint.
# Part 2: Update the Database 
  1. Add new restaurant data:
     * Add information for a new halal restaurant "Penang Flavours" in Greenwich.
  2. Find BusinessTypeID:
     * Query for the BusinessTypeID of establishments with the type "Restaurant/Cafe/Canteen".
  3. Remove establishments in Dover:
     * Query and remove any establishments in Dover from the database.
  4. Update latitude, longitude, and RatingValue:
     * Convert the latitude and longitude fields from strings to decimal numbers.
     * Convert RatingValue to integer values.
# Part 3: Exploratory Analysis
  1. Query 1: Find establishments with a hygiene score of 20.
  2. Query 2: Find establishments in London with a RatingValue of 4 or higher.
  3. Query 3: Identify the top 5 establishments with a RatingValue of 5, sorted by the lowest hygiene score, and nearest to "Penang Flavours".
  4. Query 4: Count establishments with a hygiene score of 0, grouped by Local Authority area, and display the top 10 areas. **Aggregration method was used to answer this question** 
# Requirements
* Database Setup: Correctly import data, verify database setup, and perform necessary operations (add data, remove specific documents, and update fields).
* Exploratory Analysis: Use MongoDB queries, aggregation pipelines, and Python to analyze and visualize the data.
