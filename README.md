# Coding-Assignment-Data-Curation-and-Analysis

## Project Overview

This project is designed to extract, analyze, and visualize Gross Domestic Product (GDP) data sourced from the Wikipedia page "List of countries by GDP (nominal)." The project involves web scraping using the requests and BeautifulSoup libraries to extract data and then visualizing this data using the pandas, Matplotlib, and Seaborn libraries. The main goal is to understand global economic patterns and showcase the GDP standings of various countries.

## Objectives

- **Data Extraction**: Utilize web scraping techniques via the `requests` and `BeautifulSoup` libraries to retrieve GDP data from the Wikipedia page.
- **Data Analysis and Visualization**: Employ the `pandas`, `matplotlib`, and `seaborn` libraries to process and visualize the collected data.
- **Insightful Representations**: Showcase top countries by GDP, regional GDP distributions, GDP trends over time, and estimated values from major organizations (IMF, World Bank, United Nations).

## Source Data

The GDP data is acquired from the Wikipedia page ["List of countries by GDP (nominal)"](https://en.wikipedia.org/wiki/List_of_countries_by_GDP_(nominal)). There is no need for a specific API as the data is publicly available on the Wikipedia website.

## Data Attributes

The collected data consists of several key attributes for each country or territory, including:
- **Country/Territory**: Name of the country or territory.
- **IMF Forecast**: GDP values forecasted by the International Monetary Fund.
- **IMF Year**: Corresponding year for the IMF forecast.
- **World Bank Estimate**: Estimated GDP values by the World Bank.
- **World Bank Year**: Corresponding year for the World Bank estimate.
- **United Nations Estimate**: Estimated GDP values by the United Nations.
- **United Nations Year**: Corresponding year for the United Nations estimate.

## Data Visualization

1. **Top N Countries by GDP (IMF Forecast)**: A bar plot representing the top N countries based on their GDP forecasts by the IMF.
2. **GDP by UN Region**: A bar plot displaying the total GDP for each UN region, ranked in descending order.
3. **GDP Estimates Over Time for Selected Countries**: Line plots illustrating the GDP estimates over time for selected countries, including IMF forecasts, World Bank estimates, and United Nations estimates.
4. **GDP Trends Over the Years**: A line plot showcasing the mean GDP trends over the years for IMF, World Bank, and United Nations estimates.

## Potential Issues

Wikipedia data might be prone to edits by multiple contributors, potentially introducing bias or errors. Therefore, it is crucial to cross-reference this information with other reliable sources to ensure accuracy, especially for critical applications.

## Dependencies

To run this project, you will require the following Python libraries:
- `requests`
- `BeautifulSoup`
- `pandas`
- `re`
- `matplotlib`
- `seaborn`

You can install these libraries using `pip install`.

## How the Code Works

### Step 1: Data Extraction
The code starts by importing necessary libraries such as `requests`, `BeautifulSoup`, `pandas`, `re`, `matplotlib`, and `seaborn`. It utilizes `requests.get` to fetch the Wikipedia page on GDP, and then, `BeautifulSoup` helps parse the HTML content.

### Step 2: Data Structuring
The code identifies the GDP data table on the Wikipedia page using BeautifulSoup and stores it in a structured format within a Pandas DataFrame. It cleans and organizes the data by removing unnecessary characters, converting values to numeric formats, and handling missing data. Descriptive statistics are then printed.

### Step 3: Data Visualization
#### Visualization 1: Top N Countries by GDP (IMF Forecast)
The code generates a bar plot showcasing the top N countries by GDP as forecasted by the International Monetary Fund (IMF) using the extracted and cleaned data.

#### Visualization 2: GDP by UN Region
Another bar plot is created to display the total GDP for each United Nations (UN) region, sorted in descending order based on IMF forecasted values.

#### Visualization 3: GDP Estimates Over Time for Selected Countries
Line plots are plotted for selected countries, illustrating their GDP estimates over time. The data includes forecasts by the IMF, estimates by the World Bank and the United Nations.

#### Visualization 4: GDP Trends Over the Years
A line plot is generated to showcase the mean GDP trends over the years for IMF, World Bank, and United Nations estimates.

## Summary

This project involves scraping GDP data from a Wikipedia page and utilizing Python for data curation and visualization. It aims to provide comprehensive insights into GDP trends, the top countries by GDP, and regional GDP distributions. The visualizations created aid in understanding global economic patterns and interpreting the GDP data effectively.

## Note on Data Usage

The scraped data is sourced from Wikipedia and is subject to Wikipedia's terms of use and license. Please review and adhere to these terms before using the data.
