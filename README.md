# No Search

no-search-ext is a simple Firefox Web Extension that adds a "search engine" that does nothing.

A browser address bar should never default to searching either by design or via a race condition to prevent privacy leaks in the case of human error such as in these scenarios:

- Selecting or copying a URL with an invalid URL scheme
- Accidentally mistyping the URL scheme

Fortunately Firefox is allows us to use any search engine we want in the Address Bar (or Search Bar). Unfortunately Firefox requires that a HTTP or HTTPS URL be provided as the search URL. To work around this, we use the internal ".invalid" top-level domain (TLD) as the search URL so that the search does nothing.

This extension contains the following files and will only ask to make itself the default search engine.

- manifest.json
- icon-96.png
- icon-48.png
- favicon.ico

