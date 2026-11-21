# markdown2docs

Convert markdown to .docx, .html or .pdf, or copy it formatted into Word, Google Docs or Gmail: https://delange.dev/markdown2docs

It also works the other way: switch to Docs → Markdown, paste formatted text from Google Docs, Word or a web page, or drop a .docx or .html file, then copy or download the markdown.

A single static `index.html` that runs fully in the browser, using [marked](https://github.com/markedjs/marked), [docx](https://github.com/dolanmiu/docx) and [DOMPurify](https://github.com/cure53/DOMPurify), and for the way back [turndown](https://github.com/mixmark-io/turndown) with its [GFM plugin](https://github.com/mixmark-io/turndown-plugin-gfm) and [mammoth](https://github.com/mwilliamson/mammoth.js).
A Content Security Policy blocks every request to another host.
`vendor/` holds the unmodified browser builds from the npm packages (docx, turndown, the GFM plugin and mammoth get a license header): upgrade a library by replacing its file.
Rebuilt from the [markdown2word.com](https://web.archive.org/web/20260410025511/https://www.markdown2word.com/) UX.

Run locally with `python3 -m http.server` and open http://localhost:8000.
