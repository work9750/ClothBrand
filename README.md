# Bible Verse Scanner

A simple, glassy one-page website. Every time the page loads, it shows a random Bible verse (King James Version). Tap **Show another** to see a different one.

It is built to sit behind a QR code printed on the back of a shirt, so anyone who scans it is shown a verse.

## How it works

- One file: `index.html`. No build step, no frameworks, no tracking.
- A list of verses is stored inside the page. A random one is picked on each load, and the same verse is never shown twice in a row.
- Black-and-white cherry blossom design with a frosted-glass card. It works on phones and switches to a dark look when the device is in dark mode.

## Put it online (GitHub Pages)

1. Upload `index.html` to a public GitHub repository.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose `main` and `/ (root)`, then click **Save**.
4. Your site will be live at `https://YOUR-USERNAME.github.io/REPO-NAME/`.
5. Make your QR code from that address.

## Add or change verses

Open `index.html` and find the list that starts with `const V=[`. Each verse is one line in this format:

```js
["John 3:16","For God so loved the world..."],
```

Add a new line in the same format, keep the comma at the end, and save.

## License

Released under the [MIT License](LICENSE).
