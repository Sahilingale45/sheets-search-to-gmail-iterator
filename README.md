# sheets-search-to-gmail-iterator
A Make.com automation blueprint that searches rows in a Google Sheet, iterates through the matching results, and dynamically triggers individualized emails via Gmail.
# Google Sheets Batch Search & Gmail Iterator Automation

This repository hosts a Make.com (formerly Integromat) scenario blueprint designed to batch-process spreadsheet rows and automate mass communication workflows seamlessly.

## 🚀 How It Works
1. **Fetch (Google Sheets - Search Rows):** Queries a target spreadsheet on a set schedule to find all rows that match a specific set of criteria.
2. **Loop (Iterator):** Accepts the collection of matching rows and splits them into individual items so subsequent actions can process them one by one.
3. **Execution (Gmail - Send an email):** Loops through each item produced by the iterator to construct and dispatch a tailored, data-mapped email for every record.

## 📦 What's Included
* `/blueprints/sheets-search-to-gmail-iterator.json`: The exported Make.com scenario configuration blueprint.

## 🔧 Setup Instructions
1. Open your **Make.com** account.
2. Create a new scenario, click the three dots (`...`) located in the bottom control bar, and select **Import Blueprint**.
3. Upload the `.json` configuration file provided in this repository.
4. Set up your app connections and parameters:
   * **Google Sheets:** Select your target spreadsheet, sheet name, and define your search filter options (e.g., `Status` equals `Pending`).
   * **Iterator:** Ensure it is correctly mapping the array output directly from the Google Sheets search module.
   * **Gmail:** Connect your inbox and dynamically map fields from the iterator (such as recipient email, subject headers, and body text variables).
5. Save the workflow configuration and switch the scheduling toggle to **ON**.
