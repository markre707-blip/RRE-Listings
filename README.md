# Listing Activity · Rapisarda Real Estate

A one-page public report for one listing by Tom Rapisarda, Rapisarda Real Estate. It covers:

- Showings and online activity in the latest week
- Overall totals since listing
- Showings and online activity in the first week
- How the listing compares with the team's other recent listings

## Which listing it shows

The same `index.html` works in every listing's repo. The page reads the repo name from its address (e.g. `/805AvonCt/`) and finds the matching row in the `repo` column of the Listings tab. To preview any listing, add `?listing=<listing_id>` to the address.

## Publishing a new listing

1. Create a public GitHub repo named exactly as the listing's `repo` value (e.g. `4114RowlandDr`).
2. Upload `index.html` and this README.
3. Settings → Pages → Deploy from branch → `main`, folder `/` → Save.

## Updating

The page loads its numbers from the public Google Sheet "RRE Public Listing Data" each time it's opened, so you don't need to edit or re-upload anything. A scheduled Claude task refreshes the sheet every morning, adds new active listings from Trello, and marks sold ones. Zillow/Redfin saves, list price, sqft and MLS # are entered by hand in the sheet.
