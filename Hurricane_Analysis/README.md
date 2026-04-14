Project Goals
You will work to write several functions that organize and manipulate data about Category 5 Hurricanes, the strongest hurricanes as rated by their wind speed. Each one of these functions will use a number of parameters, conditionals, lists, dictionaries, string manipulation, and return statements.

Prerequisites
In order to complete this project, you should have completed the Loops and Dictionaries sections of the Learn Python 3 Course. This content is also covered in the Data Scientist Career Path.

Project Requirements
Hurricanes, also known as cyclones or typhoons, are one of the most powerful forces of nature on Earth. Due to climate change caused by human activity, the number and intensity of hurricanes has risen, calling for better preparation by the many communities that are devastated by them. As a concerned environmentalist, you want to look at data about the most powerful hurricanes that have occured. 

1. Begin by looking at the damages list. The list contains strings representing the total cost in USD($) caused by 34 category 5 hurricanes (wind speeds 157 mph (252 km/h)) in the Atlantic region. For some of the hurricanes, damage data was not recorded ("Damages not recorded"), while the rest are written in the format "Prefix-B/M", where B stands for billions (1000000000) and M stands for millions (1000000).

Write a function that returns a new list of updated damages where the recorded data is converted to float values and the missing data is retained as "Damages not recorded".

2. Additional data collected on the 34 strongest Atlantic hurricanes are provided in a series of lists. The data includes:

    names: names of the hurricanes
    months: months in which the hurricanes occurred
    years: years in which the hurricanes occurred
    max_sustained_winds: maximum sustained winds (miles per hour) of the hurricanes
    areas_affected: list of different areas affected by each of the hurricanes
    deaths: total number of deaths caused by each of the hurricanes

The data is organized such that the data at each index, from 0 to 33, corresponds to the same hurricane.

Write a function that constructs a dictionary made out of the lists, where the keys of the dictionary are the names of the hurricanes, and the values are dictionaries themselves containing a key for each piece of data (Name, Month, Year, Max Sustained Wind, Areas Affected, Damage, Death) about the hurricane.

3. In addition to organizing the hurricanes in a dictionary with names as the key, you want to be able to organize the hurricanes by year.

Write a function that converts the current dictionary of hurricanes to a new dictionary, where the keys are years and the values are lists containing a dictionary for each hurricane that occurred in that year.

4. Knowing how often each of the areas of the Atlantic are affected by these strong hurricanes is important for making preparations for future hurricanes.

Write a function that counts how often each area is listed as an affected area of a hurricane. Store and return the results in a dictionary where the keys are the affected areas and the values are counts of how many times the areas were affected.

5. Write a function that finds the area affected by the most hurricanes, and how often it was hit.

6. Write a function that finds the hurricane that caused the greatest number of deaths, and how many deaths it caused.

7. Just as hurricanes are rated by their windspeed, you want to try rating hurricanes based on other metrics. 
Write a function that rates hurricanes on a mortality scale according to the following ratings, where the key is the rating and the value is the upper bound of deaths for that rating.

mortality_scale = {0: 0,
1: 100,
2: 500,
3: 1000,
4: 10000}

For example, a hurricane with a 1 mortality rating would have resulted in greater than 0 but less than or equal to 100 deaths. A hurricane with a 5 mortality would have resulted in greater than 10000 deaths.

Store the hurricanes in a new dictionary where the keys are the mortaility ratings and the values are lists containing a dictionary for each hurricane that falls into that mortality rating.

8. Write a function that finds the hurricane that caused the greatest damage, and how costly it was.

9. Rate hurricanes according to how much damage they cause.
Write a function that rates hurricanes on a damage scale according to the following ratings, where the key is the rating and the value is the upper bound of damage for that rating.

damage_scale = {0: 0,
1: 100000000,
2: 1000000000,
3: 10000000000,
4: 50000000000}

For example, a hurricane with a 1 damage rating would have resulted in damages greater than 0 USD but less than or equal to 100000000 USD. A hurricane with a 5 damage rating would have resulted in damages greater than 50000000000 USD (talk about a lot of money).

Store the hurricanes in a new dictionary where the keys are damage ratings and the values are lists containing a dictionary for each hurricane that falls into that damage rating.
