# Objective
The objective of this project is to clean and preprocess the WebDevelopment.csv dataset using the pandas library in Python. The dataset contains information about web development courses from different websites. The data was downloaded from Kaggle and contains 1200 rows and 16 columns.

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
- Unnamed: 11: an unnamed column that has no values
- Unnamed: 12: an unnamed column that has no values
- Unnamed: 13: an unnamed column that has no values
- Unnamed: 14: an unnamed column that has no values
- Unnamed: 15: an unnamed column that has no values

# Technologies Used
Python 3.9.7
Pandas 1.3.3

# Instructions
The following steps were taken to clean and preprocess the dataset:
- Import the necessary libraries (pandas and numpy)
- Read the WebDevelopment.csv file using pd.read_csv() and check the first five rows using df.head()
- Check the number of rows and columns using df.shape and print the results using print(df.shape).
- Investigate the data types and the number of null values in each column using df.info().
- Drop unwanted columns using df.drop() and set inplace=True to apply the changes to the dataframe.
- Clean individual columns using various pandas functions, such as str.replace(), astype(), and apply().

# Data Cleaning
The dataset was cleaned using pandas library in Python. The cleaning steps taken are:
- Dropping unwanted columns: The columns, 'Unnamed: 11', 'Unnamed: 12', 'Unnamed: 13', 'Unnamed: 14', and 'Unnamed: 15', were dropped as they contained no data.
- Standardizing values in the isPaid column: The values in the isPaid column were standardized to be either 'TRUE' or 'FALSE' to reflect whether a course is paid or not.
- Cleaning the price column: The values in the price column were transformed from strings to integers. The negative values were converted to positive values, and the 'Free' values were converted to 0.
- Cleaning the numReviews column: The negative values in the numReviews column were converted to positive values.
- Cleaning the instructionalLevel column: The values in the instructionalLevel column were standardized to be either 'All', 'Beginner', 'Intermediate', or 'Expert'.
- Cleaning the contentInfo (mins) column: The duration of the courses was converted from hours to minutes.

# Conclusion
The WebDevelopment.csv dataset was cleaned and preprocessed to prepare it for further analysis. The data cleaning process involved dropping unwanted columns, transforming the data types, replacing values, and converting the duration of the course from hours to minutes. The resulting dataset contains 11 columns with no null values. The cleaned dataset can be used for exploratory data analysis and machine learning tasks.
