## Phishing

A git for Phishing tips, tools and HTML pages.

**Created for educational purpose, phishing in the wild is illegal, except in lakes.**

### How to use

1. Choose a page in the `pages` folder and copy the HTML code to a new file (ie: `Facebook.html`)
2. By default, the credentials are sent to a `GetCreds.php` page (`scripts/GetCreds.php`):
- Put the `GetCreds.php` script into the same folder than your HTML evil page
- Replace the redirect link (`<REDIRECT-URL>`) by the real website in `GetCreds.php` (ie: `https://www.facebook.com`)
4. Host your pages online
5. Send the link and wait for the user to visit it
6. Check the results into the `logs.txt` file

### Add a keylogger

You can add a JS Keylogger to the evil page to gather credentials even if the user does not submit the authentication form:
1. Add the code from `scripts/keylogger.html` to your HTML evil page
2. Replace the `<URL>` value in the code by your HTTP request handler URL (ie: `https://webhook.site/xxxxxxxxxxxxxxxxxxxxxxx`)
3. Replace the `<USER-FIELD>` value by the name of the username field in your evil page (ie: username, user, email, ...)
4. Replace the `<PASS-FIELD>` value by the name of the password field in your evil page (ie: password, pass, secret, ...)
5. Check the incoming requests when users visit your evil page

A new request will be sent everytime the values of the authentication form changes --> when the user is typing his password
