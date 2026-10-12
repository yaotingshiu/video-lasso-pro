# Privacy Policy

Last updated: 12 October 2026

This policy explains how **Video Lasso** ("the Tool") and its official website handle data. The Tool is developed and maintained by an individual developer, Hsu Yao Ting ("the Developer", "we"). We process personal data in accordance with the laws of the Republic of China (Taiwan), including the Personal Data Protection Act ("PDPA"). By using the Tool you acknowledge this policy; terms of use are in the [Terms of Service](terms.html).

**In short:** the Tool works inside your browser. There are no accounts and no analytics, and we do not run a server that receives your browsing history or video content. The only party the Tool talks to about you is the payment platform Lemon Squeezy, and only when you activate a Pro licence key.

## 1. What we do NOT collect

- The addresses or content of pages you visit, or your searches.
- The videos, audio or subtitles you detect, download or record, or your download list.
- Your name, account, location, device identifiers, usage analytics or advertising data.
- Your card or other payment details (handled by Lemon Squeezy; we never receive them).

The Tool contains no statistics, analytics, advertising or crash-reporting service.

## 2. Data stored in your own browser

The following stays in your browser (`chrome.storage` and IndexedDB) and cannot be read by the Developer:

| Data | Purpose | Where |
| --- | --- | --- |
| Preferences (language, theme, font, preview mode, subtitle language preference, logo and icon colours) | Remember your settings | storage.local |
| Video addresses and titles detected on the current tab (temporary) | Show the list of downloadable items | storage.session (cleared when the browser closes) |
| Download progress and the last 200 download records (title, thumbnail, source page address, file name, size, time) | Show "Active" and "History" | storage.local; can be deleted in the extension |
| Access to the save folder you chose (folder handle) | Save files where you asked | IndexedDB |
| Today's clip and recording counts | Apply the free plan's daily limits | storage.local and storage.sync |
| Premium-download credit counter (credits left, next refill time) | Apply the free plan's premium-download credits | storage.local and storage.sync |
| Pro licence information (key, plan, expiry, e-mail, device name, devices in use, last verification time) | Activate and keep Pro working | storage.local |

Notes:

1. **storage.sync** is provided by your browser account (Google or Microsoft). Its content may be synchronised to your other devices signed in to the same account and stored on that company's servers. This is a browser feature that we do not control and the Developer cannot access. The Tool only puts "today's clip and recording counts" in sync, so that reinstalling does not reset the counts.
2. When you uninstall the extension, the browser deletes the local data above with it.

## 3. Data sent to others

The Tool connects outside only in these cases:

| Party | When | What is sent |
| --- | --- | --- |
| **Lemon Squeezy** (api.lemonsqueezy.com) | When you activate, periodically verify, or sign out a licence key | Licence key, device name (such as "Windows · Chrome"), instance ID; Lemon Squeezy returns the plan, expiry, purchase e-mail and devices in use |
| **The site you download from** (the server hosting the video, stream or subtitles) | When you download, preview, record or export subtitles | Requested directly by your browser, just as if you were watching the video on that site; that site sees your IP address and the request. **It does not pass through our servers.** On YouTube pages the Tool asks YouTube for the video's format list |
| **GitHub Pages** (yaotingshiu.github.io) | When you open the official website, or the browser opens the thank-you page after uninstall | Ordinary web requests (IP, browser type), processed by GitHub under its own policy |

## 4. The post-uninstall page

To free your licence slot automatically after you remove the extension, the Tool sets a "page to open after uninstall". Your licence details are carried in the `#` fragment of that address. By web standards, what follows `#` is **not** sent to GitHub's servers; the script on the page reads it only inside your browser, asks Lemon Squeezy directly to sign the device out, and then clears the fragment. If you have not activated Pro, the address contains no licence information.

## 5. Why each permission is needed

The browser permissions the Tool asks for serve its core features only:

- **All-site access, webRequest, content scripts**: find video and stream addresses and subtitle tracks on the pages you browse. The analysis is local and is not uploaded.
- **downloads, unlimitedStorage, offscreen**: save files, buffer segments and merge/convert them in the background.
- **tabCapture**: record the current tab, only when you press "Record".
- **declarativeNetRequest**: add the headers a few video requests require.
- **scripting, activeTab, tabs**: read the current tab's title and state, and fetch subtitle information on the page.
- **sidePanel, storage**: the side-panel interface and saving settings.

## 6. Notice under PDPA Article 8

1. **Collector**: the Developer, Hsu Yao Ting (individual).
2. **Purpose**: licence verification and customer service (contract or quasi-contract matters; consumer and customer management and services).
3. **Categories of data**: licence key, device name, purchase e-mail (returned by Lemon Squeezy, used for display and support); your e-mail address and message if you write to us.
4. **Period, area, recipients and method of use**: from the moment you activate the licence until you sign out, uninstall or the licence ends; the area is wherever Lemon Squeezy and your browser-account provider operate; recipients are you, Lemon Squeezy (to verify the licence) and necessary support correspondence; processed electronically. **This data lives mainly in your own browser; the Developer does not build a separate database.**
5. **Your rights**: under PDPA Article 3 you may request to inquire about or review your personal data, obtain a copy, supplement or correct it, stop its collection, processing or use, and have it deleted.
6. **Effect of not providing it**: you can skip Pro and still use the free plan; without a licence key, Pro features are unavailable.

## 7. The official website

The official website is static, hosted on GitHub Pages, and **uses no analytics or tracking tools**. It only remembers your language choice in your browser's localStorage. The checkout form is embedded from Lemon Squeezy, and the data it collects and the cookies it uses are handled by Lemon Squeezy under its own privacy policy. The pages load an open-source library from cdnjs, which may keep ordinary access logs.

## 8. Security and retention

- Licence keys are shown masked in the interface; connections to Lemon Squeezy use HTTPS.
- The security of local data depends on the security of your computer and browser account. Keep your key safe and do not post it publicly.
- We do not keep your data. If you e-mail us, the message is used only to reply and resolve your issue, and can be deleted on request afterwards.

## 9. Children

The Tool is not designed for children, and we do not knowingly collect children's personal data.

## 10. Exercising your rights and complaints

Because the data mostly lives in your own browser, you can sign out a device or delete download records in the extension, or uninstall to remove all local data. To ask whether we hold anything you sent us, or to request deletion, e-mail us. For order data held by Lemon Squeezy, please exercise your rights under its privacy policy.

## 11. Changes to this policy

We may change this policy as features or regulations change. Changes will be posted here with an updated date, and for material changes we will notify you in the extension or on the official website.

## 12. Governing law

This policy is governed by the laws of the Republic of China (Taiwan); disputes are handled as set out in Section 14 of the [Terms of Service](terms.html).

## 13. Contact

Privacy questions: [speed132454@gmail.com](mailto:speed132454@gmail.com)
