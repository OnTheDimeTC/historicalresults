ON THE DIME TIMING — OFFICIAL RESULTS EMBED v1.1

Purpose
-------
Permanent results archive for the OTD website. This is separate from Live Results
and is not affected by the 24-hour Live Results retention cleanup.

Deploy
------
Upload index.html to the GitHub Pages/site location used for Official Results.

Usage
-----
Open index.html with no query string to browse all published official events.
For a specific Past Races -> Meet -> Year page, embed:

  index.html?event=<OTD EVENT UUID>

After the Bridge publishes a race, its success dialog shows the exact event query
parameter to use. Every published race under that Event UUID appears as a tab.
Re-publishing a race replaces only that race's permanent result rows.

Notes
-----
- Uses the same Supabase project as the Bridge.
- Supports finishers plus DNF/DNS.
- Does not read or mutate temporary Live Results tables.
- Uses publishable-key-safe headers (no invalid Bearer header for sb_ keys).
