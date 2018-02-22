# ON HOLD
Dear users of my script. I didn't get allot of feedback but for the ones who did, I will be working on this script again at the beginning of April. Doing a move right now and not allot of time is set asside for scripting. I'm not abandoning this project because I'm bothered as well seeing this userscript broke so unexpectedly. Thank you for your patience!

# Youtube Subscriptions Watch Later
A userscript for adding unwatched videos from your YouTube subscriptions page to the "Watch later" playlist.

    Tested on:
    OS: macOS Sierra (Version 10.12.6)
    Browser: Google Chrome Version 60.0.3112.101 (Official Build)(64-bit)
    YouTube new Material Design layout

The script is published on GreasyFork and OpenUserJS at:  
https://greasyfork.org/en/scripts/33273-youtube-subscriptions-watch-later  
https://openuserjs.org/scripts/ackoujens/YouTube_Subscriptions_Watch_Later

# Installation

- Install TamperMonkey or GreaseMonkey extension for your browser
- Visit https://greasyfork.org/en/scripts/33273-youtube-subscriptions-watch-later and hit the Install button
- Visit YouTube (or refresh the YouTube page if it's already open)

# TODO
- Hover over icon swap
- Deliver feedback when videos are added
  - Delaying video adding on each index might deliver a cool animation
  - Pop up a prompt like the regular "Watch later" one but alter the feedback text
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
  
  # Donation
If this project helped enhancing your YouTube experience, you can always treat me to a cold one :)

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.me/ackoujens)
