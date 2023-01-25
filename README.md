This project involved cleaning data from the ´salaries´ file available from Kaggle using Python in Google colab. The dataset contains ID, role, salaries and dates of employment for Mexican Federal Workers.
Upon loading the file, it became clear there were over 1.9m data points or workers. In order to reduce loading time, the file was reduced to only those workers working in Ciudad de Mexico (n = 312,647). Upon initial exploration, it was observed that the data frame contained random capitalization, relevant columns were unnecessarily separated and column headers were not capitalized. Also, the order of the columns did not appear intuitive.
In order to clean the file, firstly, all the strings were capitalized and stripped. Were capitalization of the Spanish “De” had occurred (“Ciudad De Mexico”) the replace function was used to return this to the preferred “de” (“Ciudad de Mexico”). The columns were then renamed with capital letters and underscores. The cleaning was completed using a lambda function in each instance. Then the order of the columns was changed to the more intuitive, ID, name, role, location, salary, dates employed order. 
A function using loc was then used to return the row of employee details based on the employee ID number. The accuracy of this function was confirmed by checking the original csv file.
Next, with the clean and ordered data, a nested function with format and simple calculation was used to return a short comprehensible text utilizing relevant fields from the data based on employee ID.
Finally the data frame was converted into a cleaned csv file.
The functions used here could be used to clean the entire ‘salaries’ dataset. 
Code reviews and comments are welcomed on this project.

Dataset link https://www.kaggle.com/datasets/ivansabik/mexican-federal-government-salaries
