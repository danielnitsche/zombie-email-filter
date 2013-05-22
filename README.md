Zombie email filter
====================

An attempt at reducing email stress by moving things that don't matter out of your inbox. Rather than creating a manual filter for each service you’re subscribed to, create a single broad and no-fuss filter which says **"only show me emails sent (manually) by a real human"**.

This filter is currently very gmail specific, and as such only looks at the data that gmail exposes, and filters within the functionality that gmail offers (wildcards for example aren't supported). The filter currently matches on:

* From: no reply and bounced email addresses
* Subject: invoices/bills (when there is an attachment). Excludes all replied and forwarded emails.
* Body: standard terms seen in newsletters/notifications.

This filter isn’t perfect, but so far, catches over 90% of my zombie emails, with very few false positives (although I don’t get that many emails).

To create an zombie filter, use the conditions above, or import the XML file attached on the gmail Settings -> Filters screen.
