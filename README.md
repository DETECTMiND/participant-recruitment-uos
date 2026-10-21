# DETECTMiND Study · Participant Recruitment

Recruitment website for the **DETECTMiND study**, a joint research project by the
University of Southampton and the University of Portsmouth.

> **Study:** “A Multi-Task, Multi-Objective Decision Analytics Framework for Predicting At-Risk Mental States of Anxiety and Depression”
> **Researchers:** Anoop Kadan, Linnea Stenlund-Roderick · **ERGO number:** 117353

Live at **https://detectmind.github.io/participant-recruitment-uos/** (once GitHub Pages is enabled, see below).

## Structure

```
docs/
├── index.html      # the whole site (HTML + CSS + a little JS, no build step)
├── .nojekyll
└── assets/         # study banner, university logos, app icon, app screenshots, team photo
```

## How the form works

The site is static, so the form doesn't store anything. It checks the participant's
details, then opens a pre-written email to `detectmind@soton.ac.uk` in their own email
app. They attach their signed Consent Form and press send.

## Updating

- **Text, links, contacts:** edit `docs/index.html`. The PIS and Consent Form links point to Google Drive/Docs;
  search for `docs.google.com` / `drive.google.com` to change them.
- **Images:** replace files in `docs/assets/` with the same names.
  The university logos were cut from the study banner; swap in the official logo files when available.

Commit and push to `main`; GitHub Pages rebuilds within about a minute.

## GitHub Pages settings

Settings → Pages → **Build and deployment**
- **Source:** Deploy from a branch
- **Branch:** `main` · **Folder:** `/docs`
