# ThreadBound — public legal pages

Static hosting for ThreadBound's public-facing legal documents (GitHub Pages).

- `privacy-policy.html` — the privacy policy registered with Google Play.
- `index.html` — redirects the bare repo URL to the privacy policy.

## Do not hand-edit `privacy-policy.html`

It is a **generated** artifact. Source of truth is the ThreadBound app repo:

> `.planning/release/generated/web/privacy-policy.html`

which is itself derived verbatim from the in-app Help & Privacy copy
(`app/src/main/res/values/strings.xml`, D-68/D-69). The hosted policy and the
in-app copy must stay verbatim-identical (D-82). To change it: update the
in-app strings, regenerate in the app repo, then copy the result here.
