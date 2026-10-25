# local-json-formatter

Free browser JSON tool. Beautify, minify, validate, and repair JSON entirely on your machine — your data stays in the browser.

**Live demo:** <https://echtcosplay.de/tools/json-formatter/>

## Features

- Beautify and minify
- Validate
- Repair common broken JSON: missing quotes, single quotes, trailing commas, unclosed brackets, comments, and JSONP wrappers
- Sort keys
- Remove empty values and `null`
- Escape and unescape JSON strings

## Privacy

Formatting runs locally in a Web Worker. The page does not upload your JSON, does not ask for an account, and does not place ads on the tool.

## Use and self-host

This repository is the built static site. `index.html` is a self-contained production bundle, and `worker-DF1rjxS0.js` is the worker that bundle loads. There is no application source tree and no `package.json` here.

Serve both files from the same directory with any static host, or locally:

```bash
python -m http.server
```

Open `http://localhost:8000/`. Keep `worker-DF1rjxS0.js` beside `index.html`. The page requests that filename from the same directory.

## Chrome extension

**JSON Formatter by EchtCosplay** adds a toolbar popup, a side panel, and a right-click action that sends the current text selection to the formatter.

<https://chromewebstore.google.com/detail/json-formatter-by-echtcosplay/ikemigfmlipklfnnbaojhdkkebbpanfo>

## License

[MIT](LICENSE). Copyright 2026 echtlabs.

## Credits

Built by [EchtCosplay](https://echtcosplay.de/) / echtlabs.
