# BootCamp-Mod-8-Movies-ETL
## Overview of Project
The purpose of this project is use Jupiter Notebook to read in 3 large data files, clean the data from the files and then export the cleaned data to a SQL Database were querries can be run.

1. Jupiter Notebook was used to create an ETL function to read in the 3 data files comprising of movie and television information, such as the title, producer, country, etc.
   - Wikipedia data
   - Kaggle metadata from Movie Land's website
   - Kaggle ratings data from Movie Land's website
2. Starting with the Wikipedia data, filter out information that is not relivant to reduce the number of rows and columns of the data
   - any television shows
   - any movie without an IMDB link
   - any movie that contained null values for:
     * Box Office
     * Budget
     * Release Date
     * Running Time
3. Combine columns that contain the same information, such as "Edited by" and "Editor(s)
4. Format Budget data so that it all reads the same.
5. Moving on the Kaggle metadata and ratings data, remove any bad data that may have gotten scrambled, convert all of the data type to ensure that they are the correct type, and convert the release date to the standard datetime() format.
6. For the ratings data, convert the ratings timestamp to the datetime() format.
7. Use groupby to group the ratings to provide averages amoung the ratings from 0 to 5 in increments of 0.5.
8. Before exporting the data to SQL, all of the data tables must be merged.
9. The data is exported to SQL, where queries can be run on the data.
