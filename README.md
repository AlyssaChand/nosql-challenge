# nosql-challenge
These are the sources I used to help me write my codes: www.mongodb.com, pymongo.readthedocs.io, google, stackoverflow.com and BCS — watching our cloud recordings, using instructor activity solutions and the class activities as references.

## Part 1: Database and Jupyter Notebook Set Up
### NoSQL_setup_starter.ipynb
For this part of the challenge, I imported the establishments.json file from my terminal, named the database uk_food and the collection establishments. To confirm that the uk_food database was created and the data loaded properly I listed the databases I have in MongoDB and listed the collection in uk_food database to ensure that establishments is there. Then I found and displayed one document in the establishments collection using find_one and pprint before assigning the establishments collection to a variable.

## Part 2: Update the Database
### NoSQL_setup_starter.ipynb
For this part of the challenge, I added the following information to the database:

![image](https://github.com/AlyssaChand/nosql-challenge/assets/151655013/fc2f10ce-4ae8-44a4-84bb-826bd7cc6f1f)

I searched for the BusinessTypeID for "Restaurant/Cafe/Canteen" and updated the new restaurant with the BusinessTypeID that I found. Then I checked how many documents contain the Dover Local Authority and removed any establishments within it from the database. I checked the number of documents that contain the Dover Local Authority again to ensure they were deleted. Lastly, using update_many I converted some of the number values that were stored as strings to decimal numbers for latitude and longitude, and integer numbers for RatingValue. 

## Part 3: Exploratory Analysis
### NoSQL_analysis_starter.ipynb
For this part of the challenge, I used count_documents to display the number of documents contained in the result and used pprint to display it. Then I converted the results to a Pandas DataFrame, printed the number of rows in the DataFrame, and displayed the first 10 rows. I used the following questions to explore the database:

1. Which establishments have a hygiene score equal to 20?
2. Which establishments in London have a RatingValue greater than or equal to 4?
3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
