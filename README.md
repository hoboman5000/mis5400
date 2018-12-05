# README #

This project is for the Ritz Theater in Tooele, Utah and is being completed as coursework for Utah State University's MIS program.

API routes were written as we did to allow for the API/Data system project to be expanded to other business functions should this be successful.

Documentation will be written over the next week and is one of the remaining tasks.

What we see as the tasks left to do and a priority:
1. Make it prettier, implement CSS
2. Turn this ReadME, the help file, and other docs into the project documentation.
4. Add in some other visualizations through Tableau or some other UI
5. Python function in the API to modify the TaxRate calculation in the database if possible


Known Issues (Will be edited as resolved or new issues arise in future versions)

1. Requested Python function for editing the stored database procedures does not seem to be possible. It throws an error. Research shows that it is a limitation of pyodbc.
2. Some rounding may not be accurate for financial calculation but has been deemed adequate.

Current Version Known Major Issues:

Ability to update Employee and Feature Tables has been requested.

*******************************

Change Log
Version 8.5
1. Rewrote Box Office Reports API section to use form data and POST methods instead of passed parameters and GET methods.
2. Removed legacy Box Office Report Search and Generators.
3. Added summary statistics to the other views API.
4. Added code to require all fields be entered on Generate External Box Office API.
5. Added a script to search_records.html, search_records_temp.html, generate_bo_report.html, and all add and update record .html pages to prevent inserting negative numbers and characters in the number fields.
6. Added form reset buttons to generate_bo_report.html, search_bo_report.html, and all add and update record .html pages.
7. Changed form data types for update_feature.html and update_employee.html key fields to number from text.
8. Edited Update Employee function to require phone number and cell phone number to meet length and formatting requirements.
9. Edited all Add functions to include required fields checks.
10. Added missing messages and titles to pages.
11. Fixed all error codes.

Version 8.4
1. Consolidated Search by ID functions and html pages into 1 function and 2 pages.
2. Removed legacy search by ID routes and pages.
3. Added Search Summary Views by Range, Single Record, on field. Replaces Other Views: TotalSales, SalesByDate and CandySalesByDate API's.
4. Added date formatting function and implemented throughout code.
5. Added Search All Records Function. Replaces Get All Ticket Sales, Get all Concession Sales, Get all Employees, Get All Features, and Get all Sales.
6. Removed legacy search single records page renders.
7. User instructions added to Pages.
8. Search Pages reorganized into 1 section on UI.
9. Added Employee Contact Sheet and Manager ID look up under Employee Info.
10. Reorganized Python file to improve readability.
11. Updated API help file to reflect all new changes.

Version 8.3
1. Fixed 1000 results function in case ever needed.
2. Code clean-up from previous versions.
3. Fixed code errors in Delete functions

Version 8.2
1. All add records functions are now working.
2. Added Delete Records home page in case ever needed.

Version 8.1
1. Database netTax calculation has been fixed and is now accurately calculated and displayed.
2. Summary statistics added to Box Office Report API's (Total statistics implemented, ability to add more in future versions)
3. Bug fixes on Box Office Report API queries completed (parameterized queries needed % characters added for "like" queries)
4. get_single_bo_report parameters fixed, missing time value was corrected
5. Search by ID has been implement
6. All select functions requested by business partner are operational
7. API functions that require the passing of parameters are functional in the UI now.
8. Added navigation bar, with sub-navigation bar
9. Added theater branding
10. Added USU disclaimer
11. Added Python calculated NetPaid field to Box Office by Range API and bo_report.html
12. Added user supplied Tax Rate and Ticket Price to Box Office by Range API and bo_report.html with default values
13. bo_repot.html has been formated as requested by the business partner. Formatting was done using the API and parameters in the html file.
14. Added global variables for SALES_TAX and PRICE for ease of future update and reuse.


Version 7

1. Added completion codes to each API/Data
2. Reduces html templates to 6 through extends functionality and reuse.
3. Minor bug fixes from previous versions

Version 6
1. Implements multiple templates for html files
2. Minor bug fixes from previous versions
3. Change to API help page
4. New Default route
5. First data into html tables.


Version 5
1. Implements additional parameterized messaging to the generated html templates, "title" and "message" fields.
2. Minor bug fixes from previous versions
3. Addition of get_active_employee function
4. Removal of most JSON function from API. Some code remains for use if needed if Add Record functions are implemented.
5. Implements html templates as holding templates.

Versions 1-4
Versions 1-4 were rapid prototype versions that were proof of concept and for homework purposes only. These versions had several major flaws and were eventually partially re-written to create version 5.