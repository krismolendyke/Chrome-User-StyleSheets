# Chrome User Stylesheets

`Custom.css` can override default styles in Chrome.  It is found at `USER_DATA_DIR/User StyleSheets/Custom.css`.  Depending on your OS, `USER_DATA_DIR` can be in a [few different spots](http://www.chromium.org/user-experience/user-data-directory) in the filesystem.

I primarily use it to override styling in the Console in [Dev Tools CSS](http://codesearch.google.com/#OAMlx_jo-ck/src/chrome/tools/test/reference_build/chrome_linux/resources/inspector/devTools.css) to my liking.  For instance, I like a slightly larger font, and [my old friend Consolas](http://www.codinghorror.com/blog/2005/08/consolas-and-cleartype.html).  Obviously these are OS X specific selectors, but you get the idea.

    body.platform-mac.platform-mac-snowleopard .monospace,
    body.platform-mac.platform-mac-snowleopard .source-code {
        font-size: 12px !important;
        font-family: Consolas, monospace;
        line-height: 1.3em;
    }

