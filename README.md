# RSS-scripts
Javascript to handle multiple custom RSS feeds 

Use case: For when you have converted URLs from company job boards into custom RSS feeds in RSS.app and you want to extract specific data from each feed as JSONs into Sheets. 

This approach uses Google's Apps Script (//script.google.com) to directly pull the JSON data from each custom RSS.app URL into a Sheet built to receive it.

It ensures that the JSON data is correctly parsed and mapped to the appropriate columns in the Sheet.

Context: RSS.app allows URLs to be copied as XML, JSON and CSV so they can be extracted with little to no coding. The same process works with Airtable and other tools.

----------------------------------------------

Steps to Implement Single script for multiple feeds

1. Update the feeds Array
    - Replace {X-Site}_FEED_URL, {Y-Site}_FEED_URL, and {Z-Site}_FEED_URL with your RSS feed URLs.
    - Replace {X-Site} Tab placeholer name, {Y-Site} Tab placeholer name, etc. w/ the names of the corresponding tabs in your Sheet.
2. Set Your Spreadsheet URL
    - Replace {YOUR_SHEET_URL or other temp value} with the URL of your Sheet.
3. Run the Script
    - Open the Apps Script editor and run the fetchAllRSSJobs function.
    - Verify that each tab is populated with data from the respective feed, parsed out dicated by the script.
4. (If desired) Set Up Automation
    - Go to Triggers in Apps Script (Extensions > Apps Script > Triggers).
    - Create a time-driven trigger to run fetchAllRSSJobs periodically (e.g., hourly or daily).

Benefits of this approach
- Dynamic management: Easily add or remove feeds in the feeds array
- Centralized control: Single function handles all feeds and tabs
- Scalability: Supports any number of feeds and tabs
