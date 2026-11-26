# markdown2docs

Convert markdown to .docx, .html or .pdf, or copy it formatted into Word, Google Docs or Gmail: https://delange.dev/markdown2docs

A single static `index.html` that runs fully in the browser, using [marked](https://github.com/markedjs/marked), [docx](https://github.com/dolanmiu/docx) and [DOMPurify](https://github.com/cure53/DOMPurify).
A Content Security Policy blocks every request to another host.
`vendor/` holds the unmodified browser builds from the npm packages: upgrade a library by replacing its file.
docx ships no minified build, so its `dist/index.iife.js` goes through `npx esbuild@0.24.2 --minify` and gets a license header.
Rebuilt from the [markdown2word.com](https://web.archive.org/web/20260410025511/https://www.markdown2word.com/) UX.

Run locally with `python3 -m http.server` and open http://localhost:8000.
