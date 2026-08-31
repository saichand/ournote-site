# ournote-site

The website for Our Note, at [ournote.net](https://ournote.net/).

Static, no build step. Open `index.html` and it works.

    index.html          the landing page
    privacy/            privacy policy
    support/            support page
    ournote.css         one stylesheet, light and dark
    theme.js            shared with the other Innovatory sites
    assets/ournote/     app icon at four sizes
    CNAME               ournote.net

The palette comes from the app's own `Theme/OurNoteTheme.swift` rather than
being chosen again here, so the two cannot drift apart. Light is the default
and dark is the override, which is the opposite way round from scratchd.net.

`theme.js` stores its preference under the same key as the other sites, so a
reader who picks light on one gets light on all of them.

## Claims

Everything on these pages is checked against the app. Two worth keeping true
as the app changes:

- The privacy page says private events and ideas are hidden from the kids'
  screens but still sync to their devices, and that this is not a security
  boundary. That matches `Visibility.swift`. If a second `CKShare` for parents
  ever lands, update that section.
- The site says Our Note is in development and not on the App Store.
