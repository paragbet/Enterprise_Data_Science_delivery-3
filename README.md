# Enterprise_Data_Science_delivery-3

Author : Parag Prasad Betgeri
Matriculation No. : 419069
Description:
''' This notebook contains the defination of the various functions used in developing the Covid-19 dashboard prototype'''

- In order to visualize the COVID-19 dynamic dashboard prototype , please run " Evaluation_Walkthrough.ipynb" file.



1} In order to pull the data from source I have first defined and then called out he functions 'get_current_data_germany' and 'get_current_data_germany' in the first step of the walkthrough.

2} The data obtained in the first step of the walkthrough is then transformed to the relational data set, where the structure of the dataframe has been modified. e.g., storing the data to csv structure, changing the format of 'date' feature to datetime, renaming the columns for better data handling

3} In order for us to have the data regarding doubling rate and to have smooth data (filtered dataset) for both doubling rate as well as confirmed cases, following functions have been defined and called in the third step of the walkthrough

a} get_doubling_time_via_regression b} savgol_filter c} rolling_reg d} calc_filtered_data e} calc_doubling_rate

After application of ecery function on the dataframe the final dataframe having all the necessary data features is stored in csv structure as 'COVID_final_set'

4} In the final step of the walkthrough the 'COVID_final_set' is read to a new dataframe. Then the designing of the dynamic dashboard layout has been done with Dropdown, Markdown, lists, dictionaries etc. After the layout runs on the server showcasing the markdowns and dropdown menus, the relevent data features such as "countries, confirmed, confirmed_filtered, confirmed_DR and confirmed_filtered_DR" are assgined to the dashboard via callback function.
