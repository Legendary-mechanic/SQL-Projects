# PROJECT-1: Video Games Store Data Analysis

## Database Description
This project analyzes data from a video games store database stored in PostgreSQL format. The database contains information about the top 11,000 video games that have had the most sales of all time. It captures video game sales in North America, Europe, Japan, and other regions grouped as "Other". The database includes games from various platforms, including PC, recent consoles, and old consoles.

The sample data was obtained from a free online data source. The database consists of approximately 11,000 games, 31 platforms, 577 publishers, and 4 regions.

## Aim of the Project
The aim of this project is to analyze the video games store database using SQL queries in Python. The project explores various aspects of the database, such as game genres, publishers, platforms, sales by region, and more.

## Table Descriptions
The database consists of several tables, each serving a specific purpose. The tables and their descriptions are as follows:

### Genre
This table contains a short list of game genres, such as Strategy or Racing. It provides information about the different genres represented in the database.

### Game
This table includes a list of all the games in the database. It contains the game title and a genre_id that links to the genre table. This table does not consider the concept of a game series.

### Publisher
The publisher table represents companies that publish video games. It provides information about the publishers associated with the games in the database.

### Game_Publisher
This table serves as a joining table that defines the relationship between games and publishers. It allows multiple publishers to be associated with a game, as different publishers may work on different platforms.

### Platform
The platform table lists the different gaming platforms included in the source data. Examples of platforms in the database include PC, Playstation 3, XBOX360, and Nintendo.

### Game_Platform
This table links the games, publishers, and platforms. It provides information on which publishers released games on which platforms. By joining this table with related tables, you can obtain information about games, their publishers, and the platforms they were released on.

### Region
This table lists the four regions where sales data was captured: North America, Europe, Japan, and Others. It provides an overview of the different regions represented in the database.

### Region_Sales
The Region_Sales table records sales made for games in each region. It is the main table used for sales-related queries. The num_sales column represents the number of game sales in millions for each region.

## Project Highlights
This project showcases the ability to:
1. Connect to a PostgreSQL database using the `psycopg2` library.
2. Perform SQL queries to retrieve and analyze data.
3. Utilize the `pandas` library for data manipulation and analysis.
4. Generate insights about game genres, publishers, platforms, and sales in different regions.
5. Employ the `warnings` library to handle warnings raised during the analysis process.

## Libraries Used
The following libraries were used in this project:
- `psycopg2`: A PostgreSQL database adapter for Python.
- `pandas`: A powerful data manipulation and analysis library.
- `warnings`: A library for handling warning messages.

These libraries were essential for connecting to the database, retrieving data, performing analysis, and presenting the results.
