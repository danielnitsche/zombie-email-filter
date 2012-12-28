Inhuman email filter
====================

Having your email client notify you about email messages that you don't really care about can be infuriating. Coming up with a rule on which messages you care about can be tricky, but the best definition I've found for this rule is "only show me stuff sent (manually) by a real human". Previously, I'd set up filters for every service I'd ever subscribed to, and I'd send my emails to separate folders for each of these services. That quickly becomes a real pain to maintain, and it doesn't reduce my email stress because now I have to go through dozens of folders of unread emails. The inhuman filter is my simple attempt at solving this.

This filter is currently very gmail specific, and as such only looks at the data that gmail exposes, and filters within the functionality that gmail offers (wildcards for example aren't supported). The filter currently matches on:

* From: reply@, no-reply@, noreply@, do_not_reply@, MAILER-DAEMON@
* Subject: order without "re", invoice without "re", receipt without "re"
* Body: unsubscribe, do not reply, add our email, add our e-mail, your receipt number

This filter isn't perfect, but so far, catches over 90% of my inhman emails, with 0 false positives (although I don't get that many emails).

To create an inhuman filter, use the conditions about, or import the XML file attached on the gmail Settings -> Filters screen.
