# CMS Energy Share Volume

## Overview
This application fetches and displays the maximum and minimum common stock shares outstanding for CMS Energy from the SEC's XBRL API. It dynamically updates the displayed data based on the CIK provided in the URL query parameters.

## Setup and Installation
1. Clone the repository.
2. Open `index.html` in a web browser.

## Usage
- By default, the application displays data for CMS Energy.
- To view data for a different company, append `?CIK=XXXXXXXXXX` to the URL, replacing `XXXXXXXXXX` with the desired 10-digit CIK.

## Code Structure
- `index.html`: The main HTML file that includes the JavaScript to fetch and display data.
- The JavaScript fetches data from the SEC API and updates the DOM elements with IDs `share-entity-name`, `share-max-value`, `share-max-fy`, `share-min-value`, and `share-min-fy`.

## Functionality
- Fetches data from the SEC API using the provided CIK.
- Filters and processes the data to find the maximum and minimum share values for fiscal years greater than 2020.
- Updates the HTML elements dynamically without reloading the page.