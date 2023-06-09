Importing libraries:
The script starts by importing the necessary libraries, including webdriver from Selenium, BeautifulSoup from BeautifulSoup, pandas for data manipulation, time for adding delays, and Select from Selenium's support UI module.

IMDBScraper classc:
The script defines a class named IMDBScraper, which encapsulates the functionality of initializing the WebDriver, scraping movies, saving movie details, and closing the WebDriver.

Initializationc:
The IMDBScraper class has an __init__ method that takes the driver_path as an argument and initializes the driver_path and movie_details attributes of the class.

Initializing the WebDriver:
The initialize_driver method creates a Service object with the provided driver_path and initializes the webdriver.Edge instance, which represents the Microsoft Edge browser.

Scraping movies:
The scrape_movies method automates the process of visiting the IMDb website, performing an advanced title search, selecting search criteria, and extracting movie details. It uses the WebDriver to interact with the web page and BeautifulSoup to parse the HTML content.

Creating the DataFrame:
The to_dataframe method converts the scraped movie details stored in the movie_details list into a pandas DataFrame and saves it as a CSV file named "IMDB Movies.csv".

Closing the WebDriver:
The close method checks if the WebDriver instance exists and quits the browser if it does.

Executing the script:
The script creates an instance of the IMDBScraper class, passing the path to the Microsoft Edge WebDriver executable. It then calls the initialize_driver method to initialize the WebDriver, scrape_movies to perform the scraping, to_dataframe to save the results as a CSV file, and finally, close to quit the WebDriver.

This script automates the process of scraping movie details from IMDb, applying specific search criteria such as release date range, rating range, and movie type. It demonstrates the usage of Selenium WebDriver and BeautifulSoup to interact with web pages, extract information, and store it in a structured format.
