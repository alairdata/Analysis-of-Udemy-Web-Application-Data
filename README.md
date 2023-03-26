# Analysis-of-Udemy-Web-Application-Data
This repository contains a dataset of online web development courses available on different websites. The dataset consists of 11 columns and 1200 rows.

# Data Description
The dataset has the following columns:
- id: The unique identification number for each course.
- title: The name of the course.
- url: The website name.
- isPaid: Whether the course is paid or not.
- price: The cost of the course in USD.
- numSubscribers: The number of people subscribed to the course.
- numReviews: The number of reviews the course has received.
- numPublishedLectures: The number of lectures published in the course.
- instructionalLevel: The competency level of the course.
- contentInfo (mins): The duration of the course in minutes.
- publishedTime: The date the course was published.

# Data Cleaning
The dataset was cleaned using pandas library in Python. The cleaning steps taken are:
- Dropping unwanted columns: The columns, 'Unnamed: 11', 'Unnamed: 12', 'Unnamed: 13', 'Unnamed: 14', and 'Unnamed: 15', were dropped as they contained no data.
- Standardizing values in the isPaid column: The values in the isPaid column were standardized to be either 'TRUE' or 'FALSE' to reflect whether a course is paid or not.
- Cleaning the price column: The values in the price column were transformed from strings to integers. The negative values were converted to positive values, and the 'Free' values were converted to 0.
- Cleaning the numReviews column: The negative values in the numReviews column were converted to positive values.
- Cleaning the instructionalLevel column: The values in the instructionalLevel column were standardized to be either 'All', 'Beginner', 'Intermediate', or 'Expert'.
- Cleaning the contentInfo (mins) column: The duration of the courses was converted from hours to minutes.
