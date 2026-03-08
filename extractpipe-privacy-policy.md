# Privacy Policy for ExtractPipe

**Last Updated:** March 8, 2026

ExtractPipe ("we," "our," or "us") is committed to protecting your privacy. This Privacy Policy explains how our Chrome Extension, ExtractPipe ("the Extension"), collects, uses, and safeguards your information when you use it.

## 1. Information We Collect

ExtractPipe is designed with a privacy-first approach. We do not collect or store any of your personal data on our servers. The Extension operates entirely on your local device.

### 1.1 Data Stored Locally
The following data is collected by the Extension and stored **only locally** on your device using Chrome's local storage mechanism (`chrome.storage`):
*   **Webhook URLs:** The custom endpoint URLs you configure for sending extracted data.
*   **Custom Request Headers:** Any authorization tokens, API keys, or custom headers you define for your webhook requests.
*   **Auto-Pilot Rules:** The URL patterns (Regex/wildcards) you configure for automatic data extraction.
*   **Extension Settings:** Your preferences regarding extraction formats (Markdown/JSON) and defaults.

### 1.2 Data Processed During Use
When you activate the Extension (manually or via Auto-Pilot rules), it accesses the content of the webpage you are currently viewing to perform the extraction:
*   **Webpage Content:** The Extension uses libraries (`Readability.js` and `Turndown.js`) locally to strip ads and convert the main article body into Markdown or JSON.
*   **Webpage Metadata:** Information such as the page URL, domain, title, author, and timestamp.

This data is processed locally on your device and transmitted directly to the Webhook URL you have configured. It is **never** sent to our servers or any third-party servers other than the endpoints you explicitly specify.

## 2. How We Use the Information

The information collected and processed is used solely to provide the core functionality of ExtractPipe:
*   To extract and clean webpage content according to your settings.
*   To transmit the extracted data to your designated Webhook URLs.
*   To apply your saved Auto-Pilot rules for automated background extractions.

## 3. Data Sharing and Disclosure

We do not sell, trade, or otherwise transfer your data to outside parties. 
The only time data leaves your device via the Extension is when you explicitly instruct it to send a payload to a Webhook URL that you have configured. You are responsible for the privacy policies and security of the receiving ends of those Webhooks (e.g., Make.com, Zapier, or your custom endpoints).

## 4. Required Permissions

The Extension requests the following permissions to function correctly:
*   **`storage`**: Exclusively used to save your configurations (webhooks, headers, rules) locally.
*   **`tabs`**: Used to monitor URL changes in your browser tabs solely for matching against your existing Auto-Pilot rules.
*   **`scripting` & `activeTab`**: Used to safely inject the extraction scripts into the webpage you are viewing when an extraction is triggered.
*   **Host Permission (`<all_urls>`)**: Required to allow the Extension to extract content from any website you visit and to enable the Auto-Pilot feature.

## 5. Security

The security of your personal information and API keys is important to us. Because ExtractPipe stores your configurations locally on your device, the security of that data relies on the physical and digital security of your device and your Chrome profile. We recommend not sharing your browser profile with untrusted parties.

## 6. Changes to This Privacy Policy

We may update our Privacy Policy from time to time. We will notify you of any changes by updating the "Last Updated" date at the top of this Privacy Policy. You are advised to review this Privacy Policy periodically for any changes.

## 7. Contact Us

If you have any questions or concerns about this Privacy Policy or our practices regarding your data, please contact us through the Chrome Web Store support mechanisms.
