# Book link redirects

Live redirect behavior is managed in Cloudflare: Rules → Redirect Rules → Bulk Redirects,
list name `book-links`. This file mirrors that config as a readable reference — update both
when a destination changes.

| Path                  | Destination                                   | Title             |
|------------------------|------------------------------------------------|-------------------|
| `/book/first-call-in`  | https://youtu.be/UC-xdoxsIIo?t=757             | First Call-In     |
| `/book/second-call-in` | https://youtu.be/U3Fg3xdVuWM?t=1654            | Second Call-In    |
| `/book/launch-pitch`   | https://www.youtube.com/watch?v=yFA00zglhyc    | Launch Pitch      |

All three redirects: HTTP 302 (temporary), case-insensitive path match, works with or
without a trailing slash. `/book` itself is a static fallback page listing all three links,
in case a redirect rule is ever removed or broken.
