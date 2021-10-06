### <font color = 'navy'> Synopsis:</font>
#### Update code to check for any page 2 with more than 10 "items" or units rented out in a block. Scrape data for page 2 after scrape page 1. 
#### Added automating in selecting the earliest active month button in the calendar. Some month button options are inactivated as they are more than a year old from current month.
#### This Python code is mainly for my own code practice.
#### This Python code is used for automate in collecting rental infomation in the HDB (Housing Development Board) website.

#### The HDB website for retrieving rental information required user to key in a block number, select street name from drop down list, and select the from and to dates using its month calendar. Website will display a list of record based on the user input.

#### When user wish to get the rental information on another block in the same street, user need to click the "New Enquiry" button, website will clear all selected options and redo the same process of selections all over again.

#### This Python code will automate the selection process when user wish to get more than one block of flats' rental data, reducing time and do away the repetitive steps.

#### User just have to key in the list of block numbers/name as a form of Python list, and the correct street name as a string variable, which has to be found on the drop-down list in the website. The code will perform the selection based on the list of flats number/name and street name variable by using for loop to iterate through each flat number. At the end of each for loop, data will be consolidated by appending into a Python list. The final data will be converted to dataframe and displayed on screen.

#### > Python libraries used are:
* selenium, with Chrome as webdriver
* pandas
* time

Note on the Python code:

* The code has ability to check if there is page 2 in the website. Meaning a particular block of flat would have more than 10 units being rented out. Code does not check for page 3 and beyond as I do not expect a block with more than 20 "items".
