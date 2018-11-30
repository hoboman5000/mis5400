This project is for the Ritz Theater in Tooele, Utah and is being completed as coursework for Utah State University's MIS program.

API routes were written as we did to allow for the API/Data system project to be expanded to other business functions should this be successful.

Documentation will be written over the next week and is one of the remaining tasks.

Current Version Known Issues: The only functional portions of the UI are those that use the select all API functions. These are included in the index.html file. All functions we expected in the final project are in index_v2.html. API functions that require the passing of parameters are functional if they are passed directly, but have not been implemented in the UI. Add record functions are a low priority addition. They have been left in the API if we can implement them, but the business partner asked for the focus to be on the reporting tasks. Delete functions were left in for the same reason, but should never be implemented due to deleting records violating the database business rules.

What we see as the tasks left to do and a priority: 1. Get the UI fully functional, including the ability to pass parameterized link requests 2. Update the help file 3. Change the html structure to use less pages by using the "extends" funciton 4. Make it pretty, implement CSS and UI design 5. Write the documentation 6. Add in some other visualizations through Tableau or some other UI 7. Get the add record functions functional

We have included the current version of our API (ritz_sales_api_v2.py) along with a previous version (ritz_sales_api_v1.py) to show the changes as it has evolved. v2 is version 6 of our API at this point. The differing file names are the result of working across multiple computers, and in a group without using a resource like Github until now.
