*This is a Firefox port of the [chrome extension][original-repo-url]*

Open Spotify link in client
===========================

This is a small simple extension that tries to open any
open.spotify.com or play.spotify.com url in the Spotify desktop client
and then close the newly opened browser window.

The way the extension works is:

1. If the URL visited is open.spotify.com or play.spotify.com then
2. If the URL contains `/embed/` then don't do anything
3. Remove the FQDN part and the first slash and
4. Replace those with spotify: and
5. Replace the remaining slashes (/) with colons (:)
6. Redirect to that URL
7. Close the tab that was opening the URL if it was a newly opened tab

Available in the [Google Chrome web store][store-url]

# Changes
## 1.3
* Don't touch embedded links, so that websites that embed a playlist
  can do so without having Spotify trying to open the link automatically.
  Thanks [@shape55] for reporting the issue.

[@shape55]: https://github.com/shape55
## 1.2
* Opens links to user's playlists properly. Thanks for the bug report Robin H.

[store-url]: https://chrome.google.com/webstore/detail/open-in-spotify-client/okkdbmdhpgmajopdpmflkldkemcldnjd
[original-repo-url]: https://github.com/gaqzi/chrome-open-in-spotify-client

window by IconfactoryTeam from the Noun Project
spotify logo from page source in www.spotify.com
