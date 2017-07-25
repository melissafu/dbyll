---
layout: post
title: Scripting and MYSQL Experience
tags: [INLS161, shell, script, scripting, bash, mysql, experience, database, csv, conversion]
fullview: true
comments: true
---

**Project**

My project can be found [here](https://github.com/melissafu/melissafu-data).








**Description**

I used standard shell scripting to automate adding csv entries to a table in a database. I broke this assignment down into two scripts. 

*survey.sh*

My survey script interacts with the user to ask five general survey questions. It then takes the user's input and saves those as variables. Taking into account the date and time of the interaction, the script outputs the variables and the timestamp, along with a random number to give the entry a unique identification number, and then converts the data into a temporary csv file. This script then calls for the database script to run, and once that is finished, the temporary file is removed.

*database.sh*

After the survey script links to this database script, this script copies the temporary csv file into the secure directory that MYSQL requires the data to be in. This allows for the creation of a database and table for the entry to be put into. This script also checks for existing databases and tables to prevent creating duplicates. While doing so, it updates the user on what is occuring in the programming. Once the necessary databases and tables are created, the entry is added to the table such that the data within the entry match up with the table variables. The current version of the database is then dumped into an export file. Consecutively, the temporary csv file in the secure directory is removed, and the script prints out a confirmation message notifying the user that the entry was added to the database.

