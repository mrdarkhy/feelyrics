# Feelyrics

A transcreation player that translates song lyrics not word for word, but into the
**closest possible feeling** — *feel > meaning > words*.

**Live page:** once GitHub Pages is enabled, at `https://<user>.github.io/feelyrics/`.

## How it works
- `index.html` is a single file; there is no server and no database.
- Shared songs travel inside the `#f1.` part of the link (deflate + base64url;
  same pattern as mermaid.live and Excalidraw share links). **Lyrics are never sent to any server.**
- The only fully preloaded song is Guantanamera, whose lyrics are in the public domain
  (José Martí, 1891). Copyrighted lyrics are **never** committed to this repo — see CONTRIBUTING.

## Setup (once)
1. Push this folder to a new GitHub repo (e.g. `feelyrics`).
2. Repo → Settings → Pages → Source: `main` branch, `/ (root)` → Save.
3. The site is live within a few minutes.

## Contributing & roles (a Wikipedia-style model with zero backend)
- **Anyone:** request a song → Issue ("Song request" template); suggest a better line → Pull Request.
- **Approval:** nothing reaches the site unapproved — a maintainer reviews every PR.
- **Trusted validators:** contributors with consistently accepted PRs become *collaborators*
  and can edit directly (role ladder: Listener → Validator → Expert → Curator).

## Roadmap
- v2: split song data into `songs/*.json` (cleaner PR diffs)
- PWA manifest ("add to home screen" on phones)
- Member accounts for validators (line state machine: AI draft → suggested → settled → disputed → curator)

License: not chosen yet (repo owner's call).
