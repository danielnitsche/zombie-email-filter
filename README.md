Zombie email filter
====================

Having your email client notify you about email messages that you don't really care about can be infuriating. Coming up with a rule on which messages you care about can be tricky, but the best definition I've found for this rule is "only show me stuff sent (manually) by a real human". Previously, I'd set up filters for every service I'd ever subscribed to, and I'd send my emails to separate folders for each of these services. That quickly becomes a real pain to maintain, and it doesn't reduce my email stress because now I have to go through dozens of folders of unread emails. The zombie filter is my simple attempt at solving this.

This filter is currently very gmail specific, and as such only looks at the data that gmail exposes, and filters within the functionality that gmail offers (wildcards for example aren't supported). The filter currently matches on:

* From: no reply and bounced email addresses
* Subject: no specific, but excludes replied and forwarded emails
* Body: standard terms seen in newsletters and invoices/bills.

This filter isn't perfect, but so far, catches over 90% of my zombie emails, with very few false positives (although I don't get that many emails).

To create an zombie filter, use the conditions above, or import the XML file attached on the gmail Settings -> Filters screen.
