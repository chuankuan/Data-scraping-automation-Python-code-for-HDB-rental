### <font color = 'navy'> Synopsis:</font>
#### <font color = 'brown'> This Python code is mainly for my own practice. </font>
#### <font color = 'brown'> This Python code is used for automate in collecting rental infomation in the HDB (Housing Development Board) website.</font>

#### <font color = 'brown'>Issue: The HDB website for retrieving rental information required user to key in block number, select street name from drop down list, and select the from and to dates using its calendar. Website will display a list of record based on the user input.</font>

#### <font color = 'brown'>When user wish to get the rental information on another block in the same street, user need to click the "New Enquiry" button, website will clear all selected options and redo the same process of selections all over again. </font>

#### <font color = 'brown'> This Python code will automate the selection process when user wish to get more than one block of flats' rental data, reducing time and do away the repeitive steps.</font>

#### <font color = 'brown'> User just have to key in the list of block numbers/name as a form of Python list, and the correct street name as a string variable, which has to be found on the drop-down list in the website. The code will perform the selection based on the list of flats number/name and street name variable by using for loop to iterate through each flat number. At the end of each for loop, data will be consolidated by appending into a Python list. The final data will be converted to Pandas dataframe and print out on screen in table format. User can save the data into CSV file for future reference. </font>

#### <font color = 'brown'> Python libraries used are:
* selenium, with Chrome as webdriver
* pandas
* time

Note for the Python code:
- The website will display a maximum of 10 list of rental information in a particular flat number/name at one time. If there are more than 10 items, user need to click the "2" button option to show the next list of table. My code has so far does not cater to this additional list of table for data collection. Hence, for every flat number, there will be a maximum of 10 items in the collectd table.

* The HDB website comes with calendar for user to select particular month in interst for the data. As time past, this code may not work anymore in selecing the right month in the calendar. The calender selection portion in the code has to be updated over time by choosing the desired Xpath from the website calendar.
