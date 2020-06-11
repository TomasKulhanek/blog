# Enable Fetch to local file

If you open local file e.g. index.html, the borwser will use file:// protocol i.e. file:///C:/Projects/index.html
However any fetch request will faile due to CORS policy to allow http or https only.

To enable file: protocol to be fetched 
- in Firefox, open `about:config`and set `privacy.file_unique_origin`to `false`
- in Chrome, start with `--disable-we-security`
- or in Chrome install [Web Server for Chrome extension](https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb) which
server local files via http protocol to chrome or other browsers.
