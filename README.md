# Shipped Notes

Co-authored blog. Built with [Zola](https://www.getzola.org) v0.21.0, with a minimal terminal-style theme that lives in `templates/` and `static/style.css` and has no external dependencies.

## Write a post

1. Create `content/blog/my-post.md`:

   ```toml
   +++
   title = "My post"
   date = 2026-11-18
   description = "One line summary"
   authors = ["Çağrı"]

   [taxonomies]
   tags = ["ai"]
   +++

   Body in markdown.
   ```

2. Preview: `./serve.sh` (needs Docker), then open http://localhost:1111
3. Open a PR, get the other person's review, then merge to `main`. The site deploys automatically.

Add `draft = true` to the front matter to keep a post out of the build.

## One-time setup

- Replace `YOUR_GITHUB` / `FRIEND` in `config.toml` and `content/about.md`.
- In the GitHub repo, go to **Settings → Pages → Source** and pick **GitHub Actions**.
- Invite your co-author under **Settings → Collaborators**.
