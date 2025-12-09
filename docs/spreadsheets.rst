.. _spreadsheets: 

****************
Spreadsheets
****************

To work with all IATI data in a spreadsheet program such as Microsoft Excel or Google Sheets, you can use the `CSV Zip Download <https://tables.iatistandard.org/>`_.
You can also prepare and filter IATI data using `IATI Tables Datasette <https://datasette.tables.iatistandard.org/>`_, and download the results in CSV format. 

When working with IATI Tables data in spreadsheet programs, we recommend the following:

Disable Auto-Formatting
========================

When opening CSV files, spreadsheet programs try to automatically assign types to each column, for example for numbers and dates. 
Auto-formatting removes leading zeros from numerical identifiers, for example transforming the identifier :code:`00010` into :code:`10`.

To prevent these incorrect transformations, disable auto-formatting when loading CSV data into spreadsheets. For example, in Google Sheets, take the following steps:

1. Create an empty spreadsheet
2. Select :code:`File > Import`
3. Upload the file you want to import
4. On the :code:`Import file` screen, uncheck the box labelled "Convert text to numbers, dates and formulas"
5. Click :code:`Import data`