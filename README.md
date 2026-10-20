# DoSaS Reader Edition — four-page public site

**Status: Publisher-approved for public posting on October 20, 2026; not yet deployed.** This repository/site is distinct from the private DoSaS Author Edition and from the ChatGPT Reader Edition plugin.

## Files

- `index.html` — website/about page (`websiteURL`)
- `support.html` — support page (`supportURL`)
- `privacy.html` — privacy policy (`privacyPolicyURL`)
- `terms.html` — terms of service (`termsOfServiceURL`)
- `assets/styles.css` — local stylesheet; no Javascript, external fonts, or analytics
- `assets/dosas-reader.png` — Reader Edition's existing 512×512 icon
- `.nojekyll` — serves pages without Jekyll processing

## Publisher decisions and deployment checks

1. **Approved:** Public support address: `JoeOmega@ymail.com`. The publisher is responsible for monitoring this mailbox.
2. **Approved:** Privacy Policy and Terms of Service, both effective **October 20, 2026**. Approval was expressly confirmed by the publisher. The site is not yet public.
3. **Approved:** Support emails remain until manually archived or deleted, and archiving does not erase them. The publisher approved the Privacy Policy and Terms for publication. The publisher should update these statements if actual data-handling practices change; publication approval does not substitute for professional legal advice.
4. Preserve the approved rights attribution: the website makes no claim to rights held by another author.
5. Keep complete manuscripts, private continuity files, personal relationship chronology, raw passages, and private Author Edition materials **out of the public repository**.
6. After OpenAI approves the Reader Edition, add its actual PUBLIC chat link to `index.html`. Do not link to the private plugin page as if it were accessible to readers.

## Free GitHub Pages hosting (no new backend needed)

GitHub Pages on GitHub Free supports publishing from a **public** repository. Suggested repository name: `dosas-reader-info`.

1. Sign in to https://github.com and create a **public** repository named `dosas-reader-info` (or another name you choose).
2. Unzip the website package locally. On the new repository's **Code** tab use **Add file → Upload files**. Upload the site files **and the `assets/` directory** to the top level of the branch. Check `index.html` is at the repository root (not inside an extra enclosing folder).
3. Open repository **Settings → Pages → Build and deployment → Deploy from a branch**. Select branch `main` and folder `/(root)`, then save.
4. GitHub displays the resulting site address once the Pages deployment completes. For a project repository named `dosas-reader-info`, its typical URL pattern is `https://YOUR-GITHUB-USERNAME.github.io/dosas-reader-info/` (this is a pattern, **not a verified live URL**).
5. Open and check all four pages, the icon, mobile navigation, support contact, privacy policy and terms from an incognito browser window.
6. Only after the pages are actually live and verified, add the exact 4 HTTPS URLs to your Reader Edition's **submission-candidate** `plugin.json` under `extensions.com.openai.interface`:
   - `websiteURL`: live address ending in `/` (or `/index.html`)
   - `supportURL`: same base + `support.html`
   - `privacyPolicyURL`: same base + `privacy.html`
   - `termsOfServiceURL`: same base + `terms.html`
   Do not modify the private Author Edition or invent the URL prior to publication.

### Getting help with GitHub upload

GitHub Docs: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
Pages branch deployment: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Notes

- There is no payment integration, tracking script, contact form, ChatGPT embed, or independent DoSaS API in these files.
- GitHub may still collect access logs and other technical data under GitHub policies.
- OpenAI separately governs chats and ChatGPT account data.
- Publishing this website is **not** publishing the plugin. OpenAI submission/review remains a separate process.