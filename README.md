# Markdown Previewer

Live markdown to HTML preview with one-click copy, in a single HTML file.

**Live demo:** https://0xelitesystem.github.io/markdown-previewer/

## Use

Type markdown in the left pane. The right pane renders it as HTML in real time. Switch the right pane to "View HTML source" to read the generated markup, then copy either the markdown or the rendered HTML with the toolbar buttons. "Clear" empties the editor.

Supported syntax: ATX headings, bold, italic, strikethrough, inline code, fenced code blocks (with language hints), blockquotes, ordered and unordered lists, nested lists, task lists, links, autolinks, images, horizontal rules, and GitHub-style tables with column alignment. URLs using `javascript:`, `data:`, or `vbscript:` schemes are neutralized, and all text is HTML-escaped, so pasted content cannot inject scripts into the preview.

## Why this exists

Most online markdown editors ship your keystrokes to a server, load a megabyte of framework, or wrap a renderer in trackers and ads. This is one HTML file with an inline markdown parser. No CDN, no framework, no web font, no analytics, no network call of any kind. Open it, read every line, host it yourself. MIT licensed, so it stays yours.

## Privacy

Everything runs in your browser. Your markdown never leaves your machine. There is no server, no request, no storage, and nothing to opt out of. Copy uses the local clipboard only.

## Run locally

```
git clone https://github.com/0xelitesystem/markdown-previewer
cd markdown-previewer
```

Open `index.html` in any browser. There is nothing to install. To serve it over HTTP instead:

```
python -m http.server
```

Then visit `http://localhost:8000`.

## Build

No build step. No dependencies. The entire tool is one `index.html` with inline CSS and JavaScript.

## License

MIT. See `LICENSE`.

## Related

- https://github.com/0xelitesystem/jwt-inspector
- https://github.com/0xelitesystem/eeat-signals-reference
