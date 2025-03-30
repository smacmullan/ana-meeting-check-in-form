# ANA Meeting Check-In Form

This is a simple website for tracking attendance at meetings and other events. It features:
* Integration with Google Sheets
* Common form field names for auto-completion
* Caching information for quicker submission on subsequent meetings

## Deployment

The `public` folder must be hosted via a CDN. Common ones to use are Cloudflare Pages or GitHub Pages.

To setup:
1. Create a Google Sheet. From the menu bar, go to **Extensions** and open **Apps Script**.
2. In the **Apps Script** page, copy and paste the code from the `code.gs` file in this repository. Click the **Deploy** button on the top right and select **New Deployment**.
3. For the Apps Script deployment, select **Web App** under **Select Type**. Use your account as the **Execute as** option. Set **Anyone** as the **Who has access** option. Click **Deploy**.
4. Copy the web app link. In this repository, update the URL used by the **fetch** call in the `index.js` file to use the new web app URL.
5. Deploy the public folder to a CDN.

