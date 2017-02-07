# TEST dashboard (DRAFT version)

## Updates 06.02.2017
This version of the dashboard has the following features:

* From a user-experience perspective: if graphs are relevant for understanding outcomes and if there is no restriction in terms of available space on the site, they need to be made visible.
* A dynamic table using JQuery DataTables has been added to enable:
  * Sorting any of the columns in alphabetical order,
  * Shortening of the table by adding pagination of table entries (default number of entries per page: 50), but user can select: 25, 50 or show all entries in table,
  * Searching for table entries using a free text-format. Upon clicking the "Reset button" the search item will be cleared.
* The map showing the provinces and municipalities is automatically zoomed and positioned to fit in the 660 x 800 pixels frame, by:
  * Trimming the entries of the geojson files to only focus on the provinces and municipalities of interest.
  * Using d3's path bound function to obtain coordinates of the rectangle enclosing the targeted provinces and municipalities.
  * Automatically updating the Mercator projection's functions for centering, scaling and translating.
* The code has been commented for ongoing maintenance and allowing further improvements where needed.

## Suggestions
* Using an initialisation file enabling users to quickly update basic information in an HTML file, without the need for them to modify the HTML code. Basic information is for example:
  * Title of natural disaster,
  * Purpose of dashboard,
  * Version information,
  * Release date, and
  * Name of dashboard developer(s)
* The table header entries in the CSV data file will have spaces in their titles. These need to be adjusted manually to resemble the headers of the data table. Automate this.
* Testing of dashboard using different web browsers.

Kamal Ahmed, 06.02.207