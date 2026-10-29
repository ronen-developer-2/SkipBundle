# Privacy Policy for SkipBundle - AliExpress Direct Links

**Effective Date:** October 29, 2026  
**Last Updated:** October 29, 2026  

This Privacy Policy explains how **SkipBundle - AliExpress Direct Links** ("we", "our", or "the extension") handles user information. We are committed to protecting your privacy and ensuring transparency regarding our technical operations.

---

## 1. Single Purpose & Core Operation

SkipBundle has a single, dedicated purpose: to detect AliExpress promotional "bundle deal" redirect URLs and navigate users directly to the standalone product item page (`/item/[id].html`). 

All link parsing, URL rewriting, and redirect decisions are executed **100% locally on your device** inside your web browser.

---

## 2. Information We Do NOT Collect

We believe your browsing activity and shopping habits are strictly your business. SkipBundle:
* **Does NOT collect personally identifiable information (PII)** such as your name, email address, physical address, phone number, or government ID.
* **Does NOT monitor, log, or transmit your browsing history.** Only URLs on supported AliExpress domains are evaluated locally for bundle parameters.
* **Does NOT track what items you view, search for, or purchase.**
* **Does NOT collect financial or payment details.** Any purchase made for an optional Supporter license takes place externally on Gumroad under Gumroad’s Privacy Policy. We never access or store your credit card or payment information.
* **Does NOT use tracking cookies, analytics SDKs, or third-party advertising trackers.**
* **Does NOT sell, rent, or monetize user data under any circumstances.**

---

## 3. Data Stored Locally On Your Device

SkipBundle uses Chrome's local storage API (`chrome.storage.local`) to store minimal operational preferences directly on your computer:
* **Active State:** A boolean setting indicating whether bundle protection is currently active or paused.
* **Deals Skipped Counter:** A numeric counter tracking the number of bundle redirects avoided.
* **Recent Activity (Optional):** A list of recently bypassed item IDs (capped at 30 items) displayed in the popup for your convenience. This data never leaves your device and can be erased at any time using the "Clear" button in the extension popup.
* **Supporter Status:** A local token/license key verifying whether you have activated an optional Lifetime Supporter pass.

**None of this local data is ever transmitted to external servers.**

---

## 4. Permissions & Technical Justifications

In accordance with Google Chrome Web Store policies, SkipBundle requests only the minimum permissions necessary to function:

| Permission | Purpose |
|---|---|
| `storage` | Saves your settings (active/paused), local bypass counter, and recent history locally on your device. |
| `webNavigation` | Detects top-level bundle deal navigations on AliExpress prior to page load so you are redirected immediately without wasting bandwidth. |
| Host Permissions (`*://*.aliexpress.com/*`, `*://*.aliexpress.ru/*`, `*://*.aliexpress.us/*`) | Scoped strictly to AliExpress domains to rewrite dynamic in-page links and intercept client-side redirects. |
| Host Permission (`https://api.gumroad.com/*`) | Used solely to verify optional user-submitted license keys against Gumroad’s official license verification API. |

---

## 5. Third-Party Services

* **AliExpress:** The extension modifies AliExpress URLs locally within your browser. The extension does not transmit any data to AliExpress servers beyond your normal browser page visits.
* **Gumroad:** If you choose to purchase an optional Lifetime Supporter pass, the transaction occurs on Gumroad.com under Gumroad’s own Privacy Policy. When you enter a license key in the popup, that key is sent via HTTPS to `api.gumroad.com` solely to verify its validity.

---

## 6. Children's Privacy

SkipBundle does not knowingly collect or solicit any personal information from children under the age of 13.

---

## 7. Compliance with Chrome Web Store Policies

SkipBundle complies fully with the Google Chrome Web Store Developer Program Policies, including the User Data Policy and Limited Use Requirements:
1. The extension requests only the minimum permissions necessary to deliver its core functionality.
2. The extension does not transfer user data to third parties, broker user data, or use data for personalized advertising or creditworthiness assessment.
3. The extension contains no remotely hosted executable code.

---

## 8. Changes to This Policy

We may update this Privacy Policy from time to time to reflect extension updates or regulatory changes. Any updates will be posted in this document with a revised "Last Updated" date.

---

## 9. Contact Us

If you have questions, feedback, or concerns regarding this Privacy Policy or the extension, please open an issue on our official project repository or contact the developer directly.
