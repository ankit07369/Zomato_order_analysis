# Zomato Analysis Project

## Project Overview

Welcome to the Zomato Analysis project! This initiative employs SQL to analyze comprehensive data related to restaurants, with a focus on aspects such as restaurant names, locations, cuisines, ratings, and pricing. By utilizing SQL, we establish a robust database and a dedicated table structure, named "Zomato_Analysis" and "zomato_details" respectively, to efficiently store and manage diverse restaurant information.

## Database Setup

### 1. Create Database:

Begin by creating a dedicated database named "Zomato_Analysis" using the following SQL command:

```sql
CREATE DATABASE Zomato_Analysis;
```

After creating the database, switch to it using:

```sql
USE Zomato_Analysis;
```

### 2. Create Table:

Next, execute the SQL code below to create the "zomato_details" table, encompassing various columns to capture essential restaurant details:

```sql
CREATE TABLE zomato_details (
    restaurant_number INT,
    name VARCHAR(255),
    city VARCHAR(255),
    address VARCHAR(255),
    rating FLOAT,
    cost_per_person INT,
    cuisine VARCHAR(255),
    restaurant_link VARCHAR(255),
    menu_category VARCHAR(255),
    item VARCHAR(255),
    price FLOAT,
    veg_or_non_veg VARCHAR(10)
);
```

## Data Import

Importing data into the "zomato_details" table can be achieved through two methods:

### 1. Using LOAD DATA INFILE:

This method allows data import from a CSV file. Ensure to specify the correct file path in the SQL code and adjust field and line terminators as per the CSV file format:

```sql
LOAD DATA INFILE 'your_file_path.csv'
INTO TABLE zomato_details
FIELDS TERMINATED BY ',' 
LINES TERMINATED BY '\n';
```

### 2. Using Table Data Import Wizard:

Alternatively, a "Table Data Import Wizard" tool provides a user-friendly interface to map columns and import data from various file formats. This method simplifies the data import process, especially for non-technical users.

Choose the method that aligns with your specific requirements, ensuring the data is correctly formatted to match the table structure.

## Usage

After completing the database setup and data import, users can initiate querying and analysis of restaurant information stored in the "zomato_details" table. Utilize SQL statements to perform tasks such as filtering, sorting, aggregating, and generating insights based on the available data.

Feel free to explore the SQL code and modify it according to your specific analysis needs.

## Contributing

Contributions to the Zomato Analysis project are highly encouraged. If you encounter any issues, have suggestions, or wish to contribute improvements, please create a pull request with your changes. Your valuable input is crucial for enhancing the overall project.
