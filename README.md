# Preparing Donor Information for Salesforce

## Context
I consulted with a non-profit organization who ran a nationwide donation campaign last year. They used Google Sheets to organize information on potential donors, mark the status of contributions, and track their communication logs.

## Business Problem
After a successful fundraising campaign, the organization wanted to upload their donor list into Salesforce. The problem is that the data was far too messy to upload, making their valuable resource of donor information essentially useless. Before we worked together, the organization was planning to spend valuable volunteer hours to fix thousands of records by hand.

## Data
The data was spread across 50 tabs (one for each state), with lots of inconsistencies, errors, duplicates, and blanks. The client organization hoped to have the data combined into one tidy table in a format that would work for Salesforce and that could be referenced by volunteers making calls for next year.

I used Python and Pandas to explore the data and clean it to fit the client’s requests. You can view my process in [this Jupyter Notebook](https://github.com/amcgaha/preparing-donors-salesforce/blob/main/Cleaning%20Salesforce%20Input.ipynb).

## Product
I produced a tidy dataset for the organization, along with a few bonus features to help set them up for success in the next campaign. Because the organization uses many volunteers to make phone calls, they requested the data be organized in Google Sheets. I added the following features to their spreadsheet:

* Data validation so that volunteers editing or adding new information would be less likely to introduce errors
* Automatically generated sheets that show only records with certain statuses. For example, one sheet automatically populates with records that need to be uploaded to Salesforce, and another populates with donors who have agreed to participate.
* Conditional formatting to highlight donors who have given a decision this year
* Filter views for each state, so that there’s no need to separate states by a tab. This will also help with data integrity.

Finally, I produced a dashboard in **Power BI** to help the organization explore donor information by geography.
