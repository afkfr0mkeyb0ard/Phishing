## Phishing

A git for Phishing tips, tools and HTML pages.

**Created for educational purpose, phishing in the wild is illegal, except in lakes.**

### How to use

1. Choose a page in the `pages` folder and copy the HTML code to a new file (ie: Facebook.html)
2. By default, the credentials are sent to a `GetCreds.php` page (`scripts/GetCreds.php`):
---> Put the `GetCreds.php` script in the same folder than your HTML evil page
---> Replace the redirect link (`<REDIRECT-URL>`) by the real website in the `GetCreds.php` (ie: `https://www.facebook.com`)
4. Host your pages online
5. Send the link and wait for the user to visit it
6. Check the results into the `logs.txt` file
