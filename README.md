# RSS-scripts
Javascript to handle multiple custom RSS feeds 

Use case: For when you have converted URLs from company job boards into custom RSS feeds in RSS.app and you want to extract specific data from each feed as JSONs into Sheets. 

This approach uses Google's Apps Script (//script.google.com) to directly pull the JSON data from each custom RSS.app URL into a Sheet built to receive it.

It ensures that the JSON data is correctly parsed and mapped to the appropriate columns in the Sheet.

Context: RSS.app allows URLs to be copied as XML, JSON and CSV so they can be extracted with little to no coding. The same process works with Airtable and other tools.

