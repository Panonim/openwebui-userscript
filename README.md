# Open WebUI Message From URL Sender — Tampermonkey Userscript

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

2. **Install this userscript** by visiting the raw GitHub URL:

   ```

   ```

3. Confirm the Tampermonkey installation prompt.

---

## Development & Updating

* This script uses Tampermonkey’s automatic update mechanism.
* To update the script, simply create a pr to the GitHub repository and update the version number in the script.
* Tampermonkey checks for updates periodically or when you manually request an update.

---

## Customization

* You can adjust the delay before sending the message in the script if needed (default: 250ms).
* The script matches `localhost:3000` by default; update `@match` in the metadata if your Open WebUI runs on a different host or port.

---

## License

MIT License © \[Artur Flis]
