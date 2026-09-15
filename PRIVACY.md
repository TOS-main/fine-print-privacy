Fine Print — Privacy Policy
Last updated: 15 September 2026

This policy covers the Fine Print browser extension.

Chrome Web Store requires a privacy policy for any extension that handles user data at all, including data that never leaves your computer. This one is written to be read, not to cover anyone legally.

The short version
Fine Print reads the terms and privacy pages published by websites you visit and analyses them on your own computer.
Your browsing history is never sent anywhere. The grades and site names it remembers are stored on your machine and are never uploaded.
It never reads what you type. Not into forms, not anywhere.
The only requests that leave your computer are for documents a website already publishes — its terms, its privacy policy — and, when you ask about an extension, its public Chrome Web Store listing. Both are pages anyone can open without the extension.
There are no analytics, no trackers, no advertising, and nothing is ever sold or shared with anyone.
There is no account and no sign-in. Nothing identifies you to anybody.
What Fine Print collects and why
Sent off your device
What	When	Why	Who receives it
A request for a site's /terms, /privacy etc.	When you visit a site	To read the document and grade it	That site only. The same request your browser makes when you click the link yourself
A request for an extension's public Web Store listing	Only when you are looking at that listing, or paste its link	To show what the extension declares about your data before you install it	Google's Chrome Web Store only
A request for the developer's own website	Same moment, if their listing links to one	To grade the company's terms alongside the extension's	That developer's site only
That's the complete list. There is nothing else.

Nothing in any of those requests identifies you. They carry no account, no id, and no record of anywhere else you have been — they are ordinary requests for public pages, of the kind your browser makes whenever you open a link.

No request is ever sent to us. Fine Print has no server. There is nothing for it to phone home to.

Stored on your device, never uploaded
What	Where	Why
Grades and findings for sites you've visited	chrome.storage.local, 7-day expiry	So reopening a site is instant instead of re-fetching
A short grade history per site (last 10)	chrome.storage.local	To show whether a site's terms got worse over time
Sites and keywords you chose to watch	chrome.storage.sync	Your settings, synced by Chrome across your own devices
What Fine Print did on a site — cookies rejected, popups hidden, boxes unticked	chrome.storage.local	So the report can show it, and so you can undo it
Extensions you chose to watch, and what they last declared	chrome.storage.local	To tell you if one changes what it collects
A random install id	chrome.storage.local	Diagnostics. Random, not derived from anything about you
The grade cache and history include hostnames (like example.com) and timestamps. This is a partial record of sites you've visited, which is why it is spelled out here — but it stays on your computer, it expires after seven days, and deleting the extension deletes it.

Never collected, at all
What you type. The phone-number warning looks at a field's label to decide whether it's a phone field. It never reads the value.
Passwords, payment details, or form contents.
Your browsing history as a list sent to us.
Analytics, telemetry, crash reports, or usage statistics. There are none.
Anything for advertising. Ever.
How the cookie feature works
If you switch it on, Fine Print clicks "Reject all" on cookie banners for you, or opens the banner's settings panel, switches off every optional category and saves.

It never clicks accept. If a banner only offers "Accept", Fine Print leaves it alone for you to handle. It also never presses save on a panel it didn't change anything in, because that would just confirm whatever the site had pre-ticked.

Nothing about which banners it handled is sent anywhere. The count is kept locally so the free daily allowance works.

Clearing popups that cover the page
Off until you turn it on. When it is on, Fine Print hides things covering the page you are reading — newsletter modals, app-install prompts, survey invitations — and puts scrolling back.

Nothing is deleted. Everything is hidden, and anything hidden can be brought back three ways: the Undo in the note, the "Show what Fine Print hid" chip that stays in the corner until you use it, and the panel in the toolbar popup — which lists each hidden thing so you can bring back one without the others. Pressing Alt+Shift+X again brings it back too. You can drag the chip and the note anywhere on the screen, and Fine Print remembers where you put them.

What it will never touch, enforced in the code before anything else is considered:

Anything holding a password, card number or one-time code. A login box or a two-factor prompt looks exactly like an interstitial, and hiding one would lock you out of your own account.
The website itself. Fine Print refuses to hide anything that holds the page's own content, menu or most of its links — plenty of sites build their whole layout the same way a popup is built, and telling them apart by looks alone is not good enough.
Anything you opened yourself. Nothing is hidden within a second of a click, so dialogs you asked for stay.
Cookie banners, which the cookie feature above handles.
Image and video viewers, where the overlay is the thing you wanted.
Content behind a paywall. Fine Print will tell you a site has one. It will not get around it for you, and there is no setting that changes this.
It reads the page's layout — what is covering what, and whether a container holds a sensitive field. It does not read what you type, and nothing about which popups were cleared is sent anywhere.

The 1–100 site score
Worked out on your computer, from three things: the address itself, what the page loaded, and what the site's own terms say. Nothing is looked up and nothing is sent anywhere — which is also why it cannot tell you a site is safe. It cannot see malware or a reported phishing page. It says what it checked, and it never uses the word "safe".

What moves it: an address that reads like a brand it isn't, a domain mixing alphabets, a password or card field on an unencrypted page, a sign-in form that posts to a different domain, parts of the page loaded insecurely, how many third-party trackers the page pulls in, and the terms grade.

The tracker count is read from the page's own performance timeline — the list of things the browser already fetched. Fine Print counts the distinct third-party domains and matches them against a fixed list of known tracking services held inside the extension. Only counts and names from that list are used. No URL and no hostname from your browsing is recorded, passed on, or kept. The count is kept locally so the free daily allowance for automatic clearing works; clearing by hand is not counted at all.

Unticking pre-ticked boxes
Part of the planned paid tier, so it does not run in this version — it is described here because the code is in the extension and you can read it.

If you switch it on, Fine Print looks for checkboxes that a signup or checkout page had already ticked for you — mailing lists, "share with partners", auto-renewal — and unticks them.

The rules it follows, all of them enforced in the code:

It only ever unticks. It never ticks a box, and never submits a form.
It only touches boxes that were ticked before you arrived. Anything you tick yourself is left exactly as you left it.
It leaves required consent alone. Terms of service, privacy policy acknowledgement, age confirmation and similar are recognised and skipped — unticking those would quietly break your signup.
It tells you what it did. Silent edits to a page you are filling in would be indistinguishable from something malicious.
To decide whether a box is marketing, it reads the checkbox's own label, name, id and value — all of which are written by the website, not by you. It does not read text boxes, and there is nothing typed into a checkbox to read. Nothing about which boxes were unticked leaves your computer; only a running count is kept locally.

It is off by default, and inactive in this release.

Blocking pop-up windows
Fine Print stops windows and tabs a page opens that you did not ask for: the ad tab that appears when you click anywhere, the one that slides in behind your window as you leave, the one that fires off a timer.

To do that it has to replace window.open inside the page's own JavaScript, which is the only part of Fine Print that runs there. It looks at one thing: whether you clicked something in the last second. If you did, the window opens — which is how sign-in and card-verification windows keep working.

It does not read the page, and it does not record where the blocked window was going beyond showing you, once, so you can open it anyway if it was one you wanted.

Checking an extension before you install it
When you are looking at an extension's Chrome Web Store page — or paste its link into Fine Print — it fetches that public listing and shows what the developer has declared about your data, before you decide.

The request goes to Google's Chrome Web Store and to the developer's own site if their listing links to a privacy policy. Both are public pages. The request carries nothing about you, and no record of it is sent anywhere.

If you choose to watch an extension, Fine Print re-checks that same public listing once a day and tells you if what it declares has changed. The list of extensions you watch is stored on your computer.

Sharing
Your data is not sold, rented, or traded. It is not shared with advertisers, data brokers, or analytics companies. There are no third-party SDKs in this extension.

There is no server, no account, and no database. There is nothing held about you anywhere for anyone to ask for, sell, or lose.

A paid version, later
Fine Print is free, and everything described above is free. A paid tier is planned but is not part of this version — there is no purchase, no account and no sign-in in the extension you have.

If that changes, this policy will be updated before it ships, and Chrome will ask your permission separately for anything it needs. Nothing about how your browsing is handled would change: it would still be read on your own computer and still never uploaded.

Your choices
You want to	Do this
Stop Fine Print reading any page	Settings → Site access → Turn off. Or remove the permission in chrome://extensions
Stop all outbound requests	Settings → Local-only mode
Delete everything stored locally	Remove the extension. Chrome clears its storage
Get a copy of what is held about you	There is nothing to send. Everything Fine Print knows is on your own computer, and Settings → Export puts it in a file
There is no data deletion request to make, because there is no copy of anything anywhere else. That is not a promise about what is done with your data — it is a statement that none was taken.

Children
Fine Print is not directed at children under 13 and does not knowingly collect data from them.

Changes
If this policy changes materially, the extension's release notes will say so. The date at the top always reflects the current version.

Contact
ibweintraub@gmail.com

Questions, data deletion requests, or anything else about this policy.
