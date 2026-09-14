# Fine Print — Privacy Policy

**Last updated:** 13 September 2026

This policy covers the Fine Print browser extension.

Chrome Web Store requires a privacy policy for any extension that handles user
data at all, including data that never leaves your computer. This one is
written to be read, not to cover anyone legally.

---

## The short version

- Fine Print reads the **terms and privacy pages published by websites you
  visit** and analyses them on your own computer.
- **Your browsing history is never sent anywhere.** The grades and site names
  it remembers are stored on your machine and are never uploaded.
- **It never reads what you type.** Not into forms, not anywhere.
- The **only** thing that leaves your computer is a licence check, and only if
  you have bought Pro: your Google account id, your email address, and your
  licence key, roughly once a week.
- There are no analytics, no trackers, no advertising, and nothing is ever
  sold or shared with anyone.

---

## What Fine Print collects and why

### Sent off your device

| What | When | Why | Who receives it |
|---|---|---|---|
| A request for a site's `/terms`, `/privacy` etc. | When you visit a site | To read the document and grade it | **That site only.** The same request your browser makes when you click the link yourself |
| Google account id (`sub`), email address, licence key id | Only if you own Pro, at activation and about weekly | To tie one licence to one person and confirm a subscription is still active | Our licence server (Google Apps Script), running under the developer's Google account |

That's the complete list. There is nothing else.

We never receive your password. Google handles the sign-in and only tells us
your account id and email address.

### Stored on your device, never uploaded

| What | Where | Why |
|---|---|---|
| Grades and findings for sites you've visited | `chrome.storage.local`, 7-day expiry | So reopening a site is instant instead of re-fetching |
| A short grade history per site (last 10) | `chrome.storage.local` | To show whether a site's terms got worse over time |
| Sites and keywords you chose to watch | `chrome.storage.sync` | Your settings, synced by Chrome across your own devices |
| Your licence key and activation record | `chrome.storage.sync` / `local` | To keep Pro switched on |
| A random install id | `chrome.storage.local` | Diagnostics. Random, not derived from anything about you |

The grade cache and history include **hostnames** (like `example.com`) and
timestamps. This is a partial record of sites you've visited, which is why it
is spelled out here — but it stays on your computer, it expires after seven
days, and deleting the extension deletes it.

### Never collected, at all

- What you type. The phone-number warning looks at a field's *label* to decide
  whether it's a phone field. It never reads the value.
- Passwords, payment details, or form contents.
- Your browsing history as a list sent to us.
- Analytics, telemetry, crash reports, or usage statistics. There are none.
- Anything for advertising. Ever.

---

## How the cookie feature works

If you switch it on, Fine Print clicks "Reject all" on cookie banners for you,
or opens the banner's settings panel, switches off every optional category and
saves.

**It never clicks accept.** If a banner only offers "Accept", Fine Print
leaves it alone for you to handle. It also never presses save on a panel it
didn't change anything in, because that would just confirm whatever the site
had pre-ticked.

Nothing about which banners it handled is sent anywhere. The count is kept
locally so the free daily allowance works.

---

## Sharing

Your data is not sold, rented, or traded. It is not shared with advertisers,
data brokers, or analytics companies. There are no third-party SDKs in this
extension.

The licence data described above is processed by Google Apps Script and Google
Sheets, because that is where the licence server runs. Payments are handled by
PayPal, who have their own privacy policy; we never see your card details.

We would disclose data if legally required to, which for the licence records
would be a list of account ids and email addresses.

---

## Limited Use

Fine Print's use of information received from Google APIs adheres to the
[Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/user-data-faq),
including the Limited Use requirements.

Specifically:

- Google account data is used **only** to bind a licence to one person.
- It is not transferred to anyone except as needed for that purpose.
- It is never used for advertising of any kind.
- No human reads it except to answer a support request you send us.

---

## Your choices

| You want to | Do this |
|---|---|
| Stop Fine Print reading any page | Settings → Site access → Turn off. Or remove the permission in `chrome://extensions` |
| Stop all outbound requests | Settings → Local-only mode. Note: subscription licences need the weekly check, so this suits lifetime licences |
| Delete everything stored locally | Remove the extension. Chrome clears its storage |
| Delete your licence record | Email the address below. We delete your row from the seats list |
| Get a copy of what we hold | Email us. For almost everyone it is one row: a Google account id, an email address, and a licence id |

Fine Print works without Pro. If you never buy a licence, **nothing ever
leaves your computer** except the requests for sites' own terms pages.

---

## Children

Fine Print is not directed at children under 13 and does not knowingly collect
data from them.

## Changes

If this policy changes materially, the extension's release notes will say so.
The date at the top always reflects the current version.

## Contact

**chattbot.ai@gmail.com**

Questions, data deletion requests, or anything else about this policy.
