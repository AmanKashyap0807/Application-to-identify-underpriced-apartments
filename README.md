
# <p align="center">Building an application to identify underpriced apartments</p>
  
If you've ever searched for an apartment, you will appreciate just how frustrating the process can be. Not only is it time-consuming, but even when you do find an apartment you like, how do you know whether it's the right one?


## 🧐 Here's what I will do  
- Sourcing apartment listing data

 - Inspecting and preparing the data

 - Visualizing the data

- Regression modeling

 - Forecasting      



# <p align="center">Sourcing apartment listing data</p>
  
Most of the available data of house and apartment details are synthetic but here I am going to scrap actual data from the website 
[Renthop](https://www.renthop.com/apartments-for-rent/new-york-ny).


## 🛠️ Tech Stack
- [Python](https://www.python.org/)
- [Selenium](https://www.selenium.dev/)
- [BeautifulSoup](https://beautiful-soup-4.readthedocs.io/en/latest/)



## 🧑🏻‍💻 Detailed explaination of how data scraped

### 🛠️ Install Dependencies    
```bash
pip install selenium
from selenium import webdriver
```
        
```bash
pip install bs4
pip install html5lib
from bs4 import BeautifulSoup
```


### 🧐 Steps   
- Initialize the Microsoft Edge browser for automation using Selenium or for whatever browser you are using.
- Construct URLs: I generate target URLs for multiple pages by combining a base URL, page numbers, and a suffix.
- Extract Listings: I use Selenium to load each page and BeautifulSoup to extract the relevant HTML elements containing apartment details.
- Parse Data: I clean and process data such as the address, neighborhood, price, number of bedrooms, and bathrooms.
- Store Results: I compile the parsed data into a structured list for further analysis or use.

Repeating the above steps for different pages we will get our data for model.
        
        
        
    
        
    
        
        

  
