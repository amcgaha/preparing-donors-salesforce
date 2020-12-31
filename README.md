# Preparing Donor Information for Salesforce
I consulted with a non-profit organization to help them turn messy spreadsheets of donor information into a tidy form for importing into Salesforce. I used **Python** to clean and transform the data, and I used advanced **Google Sheets** skills to create a more robust process for data collection. Finally, I used **Power BI** to create a dashboard for my client to explore current and potential donors by geography. 

![Image](https://github.com/amcgaha/preparing-donors-salesforce/blob/main/images/yoga_explorer_preview%20-%20Copy.png)


## Context
I consulted with a non-profit organization that ran a fundraising campaign last year by partnering with yoga studios around the country. They used Google Sheets to organize information on potential partners and donors, mark the status of contributions, and track their communication logs.

## Business Problem
After a successful fundraising campaign, the organization wanted to upload their donor list into Salesforce. The problem is that the data was far too messy to upload, making their valuable resource of donor information essentially useless. Before we worked together, the organization was planning to spend valuable volunteer hours to fix thousands of records by hand.

## Data
The data was spread across 50 tabs (one for each state), with lots of inconsistencies, errors, duplicates, and blanks. The organization hoped to have the data combined into one tidy table in a format that would work for Salesforce and that could be referenced by volunteers making calls for next year.

I used **Python** and **Pandas** to explore the data and clean it to fit the client’s requests. You can view my process in [this Jupyter Notebook](https://github.com/amcgaha/preparing-donors-salesforce/blob/main/Cleaning%20Salesforce%20Input.ipynb).

## Product
I produced a tidy dataset for the organization, along with a few bonus features to help set them up for success in the next campaign. Because the organization uses many volunteers to make phone calls, they requested the data be organized in Google Sheets. I added the following features to their spreadsheet:

* Data validation so that volunteers editing or adding new information would be less likely to introduce errors
* Automatically generated sheets that show only records with certain statuses. For example, one sheet automatically populates with records that need to be uploaded to Salesforce, and another populates with donors who have agreed to participate.
* Conditional formatting to highlight donors who have given a decision this year
* Filter views for each state, so that there’s no need to separate states by a tab. This will also help with data integrity.

Finally, I produced [this dashboard](https://github.com/amcgaha/preparing-donors-salesforce/blob/main/Yoga_Studio_Preview.pdf) in **Power BI** to help the organization explore donor information by geography.
