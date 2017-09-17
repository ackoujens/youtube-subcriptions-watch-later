# Youtube Subscriptions Watch Later
A userscript for adding unwatched videos from your YouTube subscriptions page to the "Watch later" playlist.

    Tested on:
    OS: macOS Sierra (Version 10.12.6)
    Browser: Google Chrome Version 60.0.3112.101 (Official Build)(64-bit)

The script is published on GreasyFork at: https://greasyfork.org/en/scripts/33273-youtube-subscriptions-watch-later

# Installation

- Install TamperMonkey or GreaseMonkey extension for your browser
- Visit https://greasyfork.org/en/scripts/33273-youtube-subscriptions-watch-later and hit the Install button
- Visit YouTube (or refresh the YouTube page if it's already open)

# TODO
- Only add unwatched video's
- Select buttons based on aria-label to prevent other buttons with the same class to be clicked (https://blog.garstasio.com/you-dont-need-jquery/selectors/)
- Check @homepage, @homepageURL, @website and @source header elements
- Add a script icon @icon, @iconURL and @defaulticon (script icon in low res)
- Add a high res script icon (@icon64 and @icon64URL)
- Add @updateURL (version tag required)
- @downloadURL to know where the script will be downloaded when an update is detected
- @supportURL to submit issues
- Add resources with @resource for icon

Example:
```
// @resource icon1 http://tampermonkey.net/favicon.ico
// @resource icon2 /images/icon.png
// @resource html http://tampermonkey.net/index.html
// @resource xml http://tampermonkey.net/crx/tampermonkey.xml
// @resource SRIsecured1 http://tampermonkey.net/favicon.ico#md5=123434...
// @resource SRIsecured2 http://tampermonkey.net/favicon.ico#md5=123434...;sha256=234234...
```

- Research if document would run more effecient in different modes
  - @run-at document-start (injected as fast as possible)
  - @run-at document-body (when body element exists)
  - @run-at document-end (injected when or after DOMContentLoaded event was dispatched)
  - @run-at document-idle (after DOMContentLoaded event was dispatched)
