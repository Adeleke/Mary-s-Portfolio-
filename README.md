# Mary-Portfolio
# First Automation Project with Python
# Fraud Detection system- Execution Report

# INTRODUCTION
Businesses and people who conduct business online can benefit greatly from online banking transactions. The risk of losing money to fraudsters through fraudulent transactions has increased, nevertheless, as a result of the surge in financial crimes. Finding solutions to stop this threat is an increasing concern for banking and financial institutions. Based on the bank's data, this program is made to identify potentially fraudulent transactions and stop them from happening in the future. This report analyses the issue at hand and suggests potential solutions using a well designed pseudocode and flowchart that were constructed to solve the problem at hand. Additionally, it provides justifications for specific design structures, reflections on successes and difficulties.

# PROBLEM ANALYSES
The problem at hand is online frauds which has become a daily routine especially for international banks. The easiest way to understand fraudulent activities in the banking industry is to examine the fraudulent transactions and deduce characteristics that could be utilized to swiftly, possibly in real time, identify fraudulent behaviours.
It is possible to identify some characteristics of fraudulent transactions by examining past fraudulent transactions. This has led us to analyse the client (bank) dataset. We were able to deduce that the fraudulent transactions' locations are offset from the location centroid. These transactions' amounts are very different from the average transaction for the user. The descriptions of these transactions were another piece of evidence that exposed the deception. We could predict and put measures in place to double verify upcoming transactions that have these properties using statistical calculations.

# SOLUTION IMPLEMENTATION
Python is the computer programming language being used to create the application due to its ability to explore data and create machine learning models. The program is divided into four (4) modules: dataset, distance, statistics, and test, each of which contains definitions of functions that were used during the program execution. The use of functions in the implementation is intended to enable reuse and encapsulate the program from other programs. Exception handling was used to prevent the program from crashing when some of its requirements are not met.
Python is built with a variety of data structures that make it simple to process tabular data and use it for analytical purposes. In order to make each piece of information easily accessible during the data extraction process, a nested dictionary was utilized to store the dataset. User information and other lists of data that were taken from the dataset were mostly stored in list and variable data types. I ensured that I represented each data type using prefix like (var_ for variables, list_ for lists and dic_ for dictionaries) which makes them easily recognizable from a mere look at them.
The program was tested using Google Colab environment. The program was initially tested on a notebook after which they were then saved as modules so that each module could be called by the test module. The modules and dataset were saved on the google drive which was made my program path.

# PROGRAM EXECUTION
Three modules are basics used for functions definition namely; dataset_module, distance_module, and statistics_module. Their functions are accessed by the test_module which calls a menu function that was defined in the test_module itself. The program is a menu driven application that requires users to follow the prompt instructions on what options to make in order to run any of the distance or statistical function. The main menu is segmented in two which are the distance menu and the statistical menu.
The user could enter 0 to terminate the application and type within 1 14 to execute any other functions that have been defined. The dataset module is implicitly called whenever the main menu is under execution so as to access the dataset.
As a result, all the modules need to be placed in the working directory for each module to be assessable as well as the dataset itself.
PROGRAM FLOWCHART
A flowchart which could be seen as a picture of the separate steps of a process in sequential order is drawn from the viewpoint of the test_module which is the channel from which other modules functions were called or executed is depicted in the flowchart. Below is the program flowchart:

# REFLECTIONS
Firstly, I had to manually write out the formulars mathematically before thinking of writing any code, in other to give me an idea on what I want to achieve. Getting the knowledge on these statistical formulas was challenging as some of them were at the time unfamiliar to me. E.g the outliers, interquartile range, centroid etc.
After implementing these formulas I had to do a manual computation using a set of numbers to test their efficacy before calling the dataset. Based on the test carried out the functions were executing correctly. Also using a functional programming structure happens to make the work easier for me as some repeated tasks were enveloped in a function and called several times by different functions.
One challenge that I encountered was in the reading and opening of the dataset file. Opening the file was easy but saving to the dictionary was difficult as each line of record as a repeated userid which overwrite itself when saved. I overcame this challenge by using a conditional statement to determine if the user previously existed in the dictionary then add his record to the userid else add the userid along.
An interesting discovery that I got to make is understanding how to get and set working directory on google colab. I got the insight from watching a set of youtube videos and reading the documentation on google colab website. Also, I enjoyed the interactive up to date version of google colab notebook.
Given another opportunity in writing this code I would have used an object oriented programming construct to make the code shorter and more concise. Also, I would love to have used python packages where these different functions had been previously written and tested over time. This would make the program more reliable.
