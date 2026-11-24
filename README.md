# odedkovach.com

Landing page for Oded Kovach. One static file (index.html), hosted on GitHub Pages at https://www.odedkovach.com.

## How it works
- Deploy: GitHub Pages from branch main, folder /root. HTTPS enforced. The CNAME file must stay (www.odedkovach.com).
- Edit: change index.html in GitHub, commit to main, live in about a minute.
- DNS: managed in Wix (domain and Business Email subscriptions live there). A records + www CNAME point to GitHub Pages. Leave MX/TXT records alone (email).
- Design: purple gradient (#9559c5 to #2b1553), cream cards (#f4efe3), gold accents (#f2c14e), Playfair Display headline.

## Edit your links
At the top of the script in index.html there is a links object, L={...}. Anything left empty is hidden automatically.
- Filled: youtube, videos, instagram, tiktok, facebook, spotify, merch (Redbubble)
- Empty (cards hidden until filled): donate, x, appstore, googleplay
- formkey: Web3Forms public access key for the contact form (messages go to the email the key was registered with). The email is intentionally not shown on the site.

## Latest video card
Reads the channel RSS feed (channel id UCqE_iV-ZV_SJn6T89-QoN7A) through rss2json and shows the newest thumbnail and title, linking to YouTube. No embed, because embeds showed "video unavailable" (Error 153) on some computers.

## Contact form
Web3Forms (https://web3forms.com), POST via fetch, hidden honeypot field botcheck. Test by sending a message; check spam if nothing arrives.

## To do
- Add Donate, X, App Store and Google Play links when ready.
- Test the contact form end to end.
- Wix cleanup: abandoned draft site and Premium plan (renews about May 3, 2027). Keep Domain and Business Email. Do not cancel without checking.
