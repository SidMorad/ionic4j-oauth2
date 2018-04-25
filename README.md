[Original documentation](https://github.com/oktadeveloper/ionic-jhipster-starter)

Note: [issue 28](https://github.com/oktadeveloper/generator-jhipster-ionic/issues/28) explains why this repository exist.

First two commits are result of `yo jhipster-ionic` command for a JHipster application with `oauth2` authentication type. Then third commit shows migration from InAppBrowser into BrowserTab with fallback mechanism.

To see fallback mechanism, run following command:

`ionic serve`

To see BrowserTab (or InAppBrowser depends to device support) functionality, run following command:

`ionic cordova run android`

This project is configured to use `ionic4j` as it's custom-url-scheme and `ionic4j://oauth2redirect` as it's valid redirect uri. So make sure this redirect uri exist in your auth server or change it into a valid one and modify `cordova-plugin-customurlscheme` plugin with following command:

`ionic cordova plugin add cordova-plugin-customurlscheme --variable URL_SCHEME=mycoolapp`

