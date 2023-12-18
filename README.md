In this project, I employed web scraping techniques to gather meteorological data from Mars. This data was subsequently processed, visualized, and subjected to analysis using Python programming.

The project entailed the following key tasks:

Task 1: Extract headlines and introductory snippets from articles about Mars. The resulting data was optionally saved into either a JSON file or a MongoDB database.

Task 2: Obtain and interpret Martian weather information presented in tabular form.

Specific steps undertaken included:

Utilizing Splinter and Beautiful Soup to mine the Mars News website for article titles and summaries.
Compiling the extracted data into a list of dictionaries within Python.
Displaying this list within a Jupyter Notebook.
Optionally, the data was archived in a file or database, such as a JSON file or MongoDB, for easier distribution.
The designated resource for Mars Temperature Data was the webpage https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html.

The scraping targeted an HTML table encompassing data with the following headers:

id: The unique identifier for a transmission from the Curiosity rover.
terrestrial_date: The corresponding date on Earth.
sol: The sequential count of Martian days since the Curiosity rover's landing.
ls: The solar longitude.
month: The month on Mars.
min_temp: The lowest temperature recorded in Celsius for a Martian day.
pressure: The atmospheric pressure detected at the Curiosity rover's location.
Afterwards, I reviewed the data types within all DataFrame columns and converted the data to the correct datetime, integer, or float formats as needed.

The data analysis aimed to elucidate:

The total number of Martian days covered in the dataset.
Identification of the coldest and warmest months on Mars at Curiosity's location by averaging the daily minimum temperatures.
Determination of the months with the lowest and highest atmospheric pressures by calculating the average daily pressures.
Estimation of the number of Earth days in a Martian year through a graphical representation of the daily minimum temperatures.
The total count of months on Mars.
Identification of the months with the average lowest and highest temperatures and atmospheric pressures.
A visual estimation of the number of Earth days within a Martian year, striving for an accuracy within 25%.
The project utilized the following tools and technologies:

Python
JSON for data formatting
MongoDB for database management
Beautiful Soup for HTML parsing
Splinter for web automation
Matplotlib for creating visualizations
Pandas for data manipulation
Jupyter Notebook as the development environment
