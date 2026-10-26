# lunon-site-assets

Static assets for lunon.ai that need a public URL outside Framer.

- `ashby/lunon-ashby-embed.css`: the Lunon theme for the Ashby application form embedded in the lunon.ai Apply drawer. It's served through jsDelivr, pinned to a commit, and that exact URL is allowlisted in Ashby under Admin → Theme (Job Board) → Allowed Custom CSS URLs. Ashby matches the URL exactly and stores it lowercased (`lunonai`), so use the lowercase form everywhere. After you change the file, allowlist the new commit URL in Ashby and update `ASHBY_CSS_URL` in the Framer `Apply_Drawer.tsx` code file.
