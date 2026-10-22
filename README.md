# Ampvox Academy landing page

A single static page. No build step.

## Files
- index.html: the whole page (styles, scripts and images are inside it)
- og-academy.png: share image used when the link is pasted into WhatsApp, LinkedIn, etc.
- robots.txt

## Deploy on GitHub Pages
1. Create a repo and add these files to the root (or the folder you will serve).
2. Settings > Pages > Deploy from a branch > main > /root.
3. Settings > Pages > Custom domain: academy.ampvox.co.uk (or your chosen address), then add the CNAME record at your DNS host.
4. In index.html, search for `og-academy.png` and change the two share image URLs to wherever you host that file.

## Make the sign up forms save emails
1. Create a free form at formspree.io that emails blair@ampvox.co.uk.
2. In index.html, search for `SIGNUP_ENDPOINT` and set it to the form URL, for example:
   var SIGNUP_ENDPOINT='https://formspree.io/f/xxxxxxxx';
3. Until this is set, the forms show a "not switched on" message.

## Edit
- Launch date: search for `Date.UTC(2026,10,1` (months start at 0, so 10 is November).
- Fonts load from Google Fonts and the 3D scene from cdnjs, so the page needs internet.
