# Oxford Capoeira Society Agents

This repository is the root of a static website for Oxford Capoeira Society.

- Publish through GitHub Pages from the repository root.
- Repository: `https://github.com/danielhuggins/oxford-capoeira-angola`.
- Expected GitHub Pages URL: `https://danielhuggins.github.io/oxford-capoeira-angola/`.
- Keep the project flat: do not create a nested project folder or duplicate root directory.
- Use standard static hosting conventions: `index.html`, separate CSS, and separate image assets.
- Do not add a build step. The site should remain directly publishable as static files.
- Even when instructions are in Spanish, keep `agents.md` files and core HTML/CSS names in English.
- Prefer simple, maintainable HTML and CSS unless a future task clearly needs more.
- This site will be developed with AI assistance, so keep changes easy to inspect and explain.

## Architecture

The fundamental architectural constraint is "keep it simple, stupid" above all
else. Good practice should mean practical, understandable, and easy to maintain
for a small community website. The visuals can be polished and attractive, but
that should not require a build pipeline or unnecessary tooling.

## Publishing Cycle

Treat commits as a way to save work and create useful checkpoints. Remind
Mauricio to commit regularly after each reasonable chunk of work so progress can
be reviewed, compared, or recovered later.

For this site, pushing to the publishing branch corresponds to publishing the
website. Do not treat `git push` as just a backup step when working on `main`;
it should mean the current site is ready to go live through GitHub Pages.

## Local Development

Agents should expect to use Git and GitHub CLI for normal repository access.
Authenticate with GitHub CLI when needed, then use the configured repository
remote for pull, commit, and push operations.

For local preview, serve the repository root with:

```powershell
python -m http.server 8000
```

Then open `http://localhost:8000`. This server does not auto-refresh the
browser, but it serves saved file changes immediately. After editing HTML, CSS,
or image assets, remind non-technical users to save the file and refresh the
browser page to see the update. The server usually does not need to be restarted.

## User Support

Expect more than one person to work with the AI assistant, with mixed levels of
technical confidence.

When working with non-technical users, check in about consequences and explain
what is happening, why it matters, and what the practical choices are. Be
proactive about offering useful options from available capabilities, such as
previewing locally, taking screenshots, checking the live GitHub Pages site,
making small commits, comparing changes, or improving copy and layout. Take
enough time to choose sensible architecture and good practice, but define good
practice by practicality: this is a small community website, not a major
long-term software project. Maintain a minimum amount of structure so the site is
easy to update, understand, and publish.
