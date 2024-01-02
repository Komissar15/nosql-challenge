Eat Safe, Love - Analysis of UK Food Ratings

Overview:
The analysis conducted for the food magazine "Eat Safe, Love" focused on the UK Food Standards Agency's hygiene ratings. This readme outlines the setup of the database, data import, and exploratory analysis conducted using a Jupyter Notebook.

Part 1: Database and Jupyter Notebook Setup

Database Creation and Data Import:

Imported data from establishments.json into a MongoDB database named uk_food and a collection named establishments.
Included the terminal command for data import in a markdown cell within the Jupyter Notebook.
Library Import and MongoDB Connection:

Imported necessary libraries such as PyMongo for MongoDB interaction and Pretty Print (pprint) for data display.
Created an instance of the Mongo Client.
Database Confirmation:

Confirmed the existence of the uk_food database by listing databases in MongoDB.
Ensured the presence of the establishments collection within the database.
Displayed one document from the establishments collection using find_one and pprint.
Assigned the establishments collection to a variable for further use.
Part 2: Update the Database

Modifications to the Database:

Added information for a new halal restaurant, "Penang Flavours," in Greenwich, which was unrated.
Identified the BusinessTypeID for "Restaurant/Cafe/Canteen" and updated the new restaurant accordingly.
Removed establishments within the Dover Local Authority.
Data Type Conversion:

Utilized update_many to convert latitude and longitude to decimal numbers.
Employed update_many to convert RatingValue to integer numbers.
Part 3: Exploratory Analysis

Performed exploratory analysis to answer specific questions from "Eat Safe, Love":

Establishments with Hygiene Score 20:

Displayed establishments with a hygiene score of 20, providing count, the first document, and a Pandas DataFrame.
High-Rated Establishments in London:

Showcased establishments in London with a RatingValue greater than or equal to 4, presenting count, the first document, and a Pandas DataFrame.