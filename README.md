# Boxing Web Scrape Data

#### By Jarret Jeter

#### This project extracts data from boxrec such as boxer information(all boxers? boxers from select amount of countries?) to gain insights (the average fighter’s career length and amount of fights, anything else interesting I can think of)

## Rough Draft

### MVP

* elt
* table of boxers
* data visualizations

### Stretch Goals

* airflow
* table of events
* front end page?

### Technologies Used

* python
* pandas
* beautifulsoup
* cloudscraper
* google bigquery
* google data studio

## Description

The project relies first and foremost on cloudscraper and Beautifulsoup to parse data extracted from the search results of fighters on boxrec. Unfortunately I am unable to automate the search process because of the site's antibot technology, so I must manually log in first. After getting access, I create a soup object with Beautifulsoup to parse the table row html tags to find information(fighter id, name, country, etc). The specific data is then used by small functions that are called on by a larger function to create a dataframe out of the collected data. Afterwards there is some cleaning involved before saving to a csv file and loading into BigQuery. This was my first real effort at web scraping and it was very difficult narrowing down what I wanted from the unstructured data.

## Setup/Installation Requirements

* _This is a great place_
* _to list setup instructions_
* _in a simple_
* _easy-to-understand_
* _format_

_{Leave nothing to chance! You want it to be easy for potential users, employers and collaborators to run your app. Do I need to run a server? How should I set up my databases? Is there other code this application depends on? We recommend deleting the project from your desktop, re-cloning the project from GitHub, and writing down all the steps necessary to get the project working again.}_

## Known Bugs

* _Any known issues_
* _should go here_

## License

_{Let people know what to do if they run into any issues or have questions, ideas or concerns.  Encourage them to contact you or make a contribution to the code.}_

_Copyright(c) 07/28/2022 Jarret Jeter_
