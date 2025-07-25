# Open WebUI Message From URL Sender — Tampermonkey Userscript

<p>
   <img alt="Greasy Fork Downloads" src="https://img.shields.io/greasyfork/dt/542330">
   <img alt="Greasy Fork Rating" src="https://img.shields.io/greasyfork/rating-count/542330">
</p>

Automatically inject and send a message in your Open WebUI instance via URL parameters.

---

## Overview

This userscript lets you pre-fill and send a message automatically in Open WebUI by adding a `message` parameter in the URL. For example:

```
http://localhost:3000/?temporary-chat=true&model=gemma3:12b&message=Hello%20World
```

When you open the URL with this script installed, it will:

* Detect the `message` parameter
* Insert it into the chat input
* Trigger sending the message automatically

---

## Installation

1. **Install Tampermonkey** in your browser (Chrome, Firefox, Edge, etc.) if you haven’t already:
   [https://www.tampermonkey.net/](https://www.tampermonkey.net/)
2. **Go to greasy fork** https://greasyfork.org/en/scripts/542330-open-webui-message-fetcher-from-url
4. **Click** `Install this script` and on TamperMonkey choose `Install`
3. That's it! Your script should be ready to go.

---

## Development & Updating

* This script uses Tampermonkey’s automatic update mechanism.
* To update the script, simply click `Check for userscript updates` and TM will do the rest for you. 
* Tampermonkey checks for updates periodically or when you manually request an update.

* If you want to help with script development, fork the repo and create a PR wich changes. We will manually update the version number for you.

---

## Customization

* You can adjust the delay before sending the message in the script if needed (default: 250ms).
* The script matches `localhost:3000` by default; update `@match` in the metadata if your Open WebUI runs on a different host or port.

---

## License

MIT License &copy; 2025 Artur Flis
