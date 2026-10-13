# virginriverdental.com

Static website for Virgin River Dental (St. George, UT), served by GitHub Pages.

This branch is the **preview** build for virgin.elevatepractices.com: it is set to `noindex` and `robots.txt` blocks crawlers, and analytics are off, so it cannot compete with the live site in search.

- Every old WordPress URL keeps its path, title, meta description and canonical (canonicals point to virginriverdental.com).
- `/book/` forwards to online booking (new patients); `/vote/` forwards to the Best of Southern Utah ballot.
- GoHighLevel (LeadConnector) chat widget is on every page; Privacy Policy and Terms include the texting terms needed for A2P.

## Launch checklist
1. Swap in the production build (indexable, with GTM/GA) and change `CNAME` to `virginriverdental.com`.
2. Settings > Pages: Source = Deploy from a branch, Branch = main / root. Custom domain = virginriverdental.com.
3. Point DNS to GitHub Pages: A records 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153 and CNAME www -> elevate-practices.github.io.
4. When the certificate is ready, tick "Enforce HTTPS".
5. Check: home, a service page, /book/, the chat bubble, booking links.
6. Submit https://virginriverdental.com/sitemap.xml in Google Search Console.
7. Cancel the old WordPress hosting only after the new site is live and checked.
