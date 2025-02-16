# API Link Generator for one-digitalservice.ch Transaction Reports

## Description

This is a static HTML page that helps generate API links for retrieving transaction reports from `https://api.one-digitalservice.ch/v1/reports/cards/cardId/transactions`.

The page provides a user interface to input:

*   **Card ID:** The identifier for the card.
*   **Date From:** The start date for the transaction report range.
*   **Date To:** The end date for the transaction report range.

Based on these inputs, the page generates a table of links. Each link corresponds to a monthly interval within the specified date range, pointing to the API endpoint for transaction reports for that month.

## Features

*   **User-friendly Input Fields:**  Provides input fields for Card ID, Date From, and Date To.
*   **Monthly Link Generation:** Automatically generates API links, breaking down the provided date range into monthly chunks.
*   **Table Display of Links:** Presents the generated links in a clear table format, showing the month and the corresponding API link.
*   **"View Link" Functionality:** Each row in the table contains a "Link" which, when clicked, opens the API endpoint URL in a new browser tab.
*   **Login Button:** Includes a "Login" button in the header that opens the login page for `one-digitalservice.ch` in a new tab, for user convenience in accessing the service.
*   **Date Range Handling:**
    *   Accepts date ranges longer than a month.
    *   Generates links covering full months or specific date ranges within a month as needed.
    *   Uses UTC dates to ensure consistency in API requests.

## How to Use

1.  **Save the HTML file:** Save the provided HTML code as a file named `index.html` (or any name with the `.html` extension).
2.  **Open in a Web Browser:** Open the `index.html` file in your web browser (e.g., Chrome, Firefox, Safari, Edge). You can do this by double-clicking the file or dragging it into your browser window.
3.  **Enter Card ID:** In the "Card ID" field, enter the specific Card ID for which you want to generate transaction reports.
4.  **Select Date Range:** Use the "Date From" and "Date To" date pickers to select the desired start and end dates for your report.
5.  **Click "Generate Links":** Click the "Generate Links" button.
6.  **View Generated Links:**  A table labeled "Generated Links" will appear below the button. Each row in the table represents a month within your specified date range.
7.  **Open API Link:** In the "Link" column of each row, click the "Link" text. This will open the corresponding API endpoint URL in a new browser tab. You can then view the raw JSON response from the API in that tab.

## Important Notes

*   **Static HTML Page:** This is a client-side application built as a static HTML page with JavaScript. No server-side component is needed to run this tool.
*   **Client-Side Link Generation:** All link generation and processing are done in your web browser using JavaScript.
*   **Monthly Link Intervals:** The tool automatically breaks down date ranges into monthly intervals. If you provide a date range spanning multiple months, you will get separate links for each month (or partial month at the start and end of the range).
*   **UTC Dates:** The generated API links use dates formatted in UTC (Coordinated Universal Time) to ensure consistency when interacting with the API.
*   **"Login" Button:** The "Login" button is provided as a convenience to quickly access the login page of `one-digitalservice.ch` in a separate tab, in case you need to log in to access the API or related services.
*   **No Download Functionality:** The download data functionality has been removed in the latest version for simplicity. This version only generates and displays the API links for viewing in the browser.

## Disclaimer

This tool is provided as a simple, static HTML page for generating API links. It is intended for basic use and convenience.

*   **Security:** As a static, client-side tool, avoid embedding sensitive credentials directly in the HTML or JavaScript code if you intend to share or host this page in a public or less secure environment.
*   **API Terms of Service:** Ensure you comply with the terms of service and usage guidelines of `api.one-digitalservice.ch` when using the generated links and accessing their API.
*   **Error Handling:** Basic error handling (like alerts for missing inputs or invalid date ranges) is included, but more robust error handling might be needed for production use.

Feel free to modify and customize this HTML page further to suit your specific needs.