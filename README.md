ChatGPT said:
🧭 Multi-Site Jumper — README.md

File: multi-site-jumper.html
Type: Single HTML file (contains HTML + CSS + JS)
Purpose: Quickly browse through multiple website links from a single page.

🚀 Overview

Multi-Site Jumper is a stand-alone, browser-based tool that helps you open and preview multiple websites from one interface — ideal for checking username profiles (like Sherlock results), social media pages, or any list of URLs.

You paste your list of websites, hit Load, and then easily navigate through them using buttons or keyboard shortcuts.

✨ Features

✅ Paste multiple URLs (one per line).
✅ Click Load to generate a navigable list.
✅ Browse sites using:

Next / Prev buttons

Open in New Tab button
✅ Search bar to filter URLs instantly.
✅ Keyboard shortcuts:
| Key | Action |
|-----|---------|
| / | Focus the search box |
| n | Jump to next site |
| p | Go to previous site |
| o | Open current site in a new tab |
✅ URLs are saved in LocalStorage — reloading the page won’t lose your list.
✅ Smart Fallback: if a website blocks embedding in an iframe, it shows a friendly “Preview Unavailable” message with a clickable button — so you never see a blank “No site loaded” screen again.

⚙️ How It Works

The app uses an iframe to preview websites directly inside the same page.

Some websites use headers like:

X-Frame-Options: SAMEORIGIN
Content-Security-Policy: frame-ancestors 'none';


These prevent loading inside iframes (for security reasons).

When this happens, the app automatically detects it and shows a safe preview message + link instead.

📋 Usage

Create a new file named multi-site-jumper.html.

Paste the full HTML/CSS/JS code I provided earlier into it.

Save and open it in your browser (double-click the file).

Paste your list of URLs (one per line) → click Load.

Use Next, Prev, or keyboard shortcuts to navigate.

💡 Notes

100% client-side — no backend, no API keys, nothing stored online.

Works offline once loaded.

LocalStorage saves your URL list only in your browser.

For websites that don’t allow embedding, just click “Open in new tab”.

🧱 Example Use Cases

Viewing Sherlock username search results.

Checking multiple profile pages quickly.

Testing or comparing a list of domains or subdomains.

Rapidly switching between project dashboards or documentation links.
