# Installation

Minimal-StartPage is a single web page. There is nothing to build, compile or install: you only need a web browser. Pick the option that suits you.

## Option 1: use the online version (easiest)

1. Open [https://start.soholocal.nl/app](https://start.soholocal.nl/app).
2. Make it your homepage. Look for **Homepage** or **Home** in your browser's settings and enter that address.
3. On a phone, open the page in Safari (iPhone) or Chrome (Android) and add it to your home screen:
   - **iPhone:** tap the Share button, then **Add to Home Screen**.
   - **Android:** tap the three dots, then **Add to Home screen**.

This needs an internet connection, but nothing else.

## Option 2: install a copy on your computer

Use this if you want to change the page yourself, or to run a local copy. You do not need admin rights. The page uses a root base URL (`<base href="/">`), so opening `index.html` with a `file://` double-click will not load the CSS, scripts or wallpapers. Serve the folder with a local web server instead (or use Wrangler, as in Option 3).

**Step 1: download the files.** Go to the [releases page](https://github.com/a4ds5t/start.soholocal/releases/latest) and click **Source code (zip)** under the latest release. That is the tested, stable version. (The green **Code** button on the main page also has a **Download ZIP**, which gives the newest version, but that one may not be released yet.)

**Step 2: unzip the file.**
- **Windows:** right-click the downloaded ZIP and choose **Extract All…**.
- **macOS:** double-click the file. A folder appears next to it.

Move the folder somewhere you will keep it, for example your Documents folder. Keep everything inside it together: the `assets` folder must stay next to `index.html`.

**Step 3: serve the folder and check that it works.** From inside the folder, start a local server, for example:

```bash
npx --yes serve -l 8080
```

Or, with Node 22+ and the repo's Wrangler setup: `npm install`, then `npm run dev` (serves the Worker locally; the app is at `/app`).

Open the address the server prints. With a plain static server from the folder root that is usually `http://localhost:8080/` (which serves `index.html`). With Wrangler (`npm run dev`) the app is at `http://localhost:8787/app` by default. You should see the wallpaper and the clock. The quote is off by default; switch it on in the settings if you want it.

**Step 4: copy the address.** Select the address from the browser's address bar and copy it. It should start with `http://localhost` (or another local host name), not `file:///`.

**Step 5: set it as your homepage.** Paste the address into your browser's homepage setting:
- **Chrome or Edge:** open Settings, search for "homepage", turn on the home button, and choose to enter a custom web address.
- **Firefox:** open Settings, go to **Home**, and under **Homepage and new windows** choose **Custom URLs**.
- **Safari (Mac):** open Settings, go to **General**, and paste the address in the **Homepage** field.

The exact menu names can differ per browser and version. If you cannot find the setting, search the browser's settings for "homepage".

### Updating a copy

Download the ZIP again and replace the old folder with the new one. Your choices (search engine, theme, wallpaper, clock and date format) are stored in your browser, so they stay.

### Troubleshooting

- **No wallpaper, or a page without styling:** you opened `index.html` as a `file://` URL, or the `assets` folder (or other files) is missing or was moved. Serve the folder over `http://` as in step 3, keeping all files together.
- **The homepage shows an error:** the address is probably wrong. Repeat step 4 and paste the new address.
- **You still see an old version:** refresh the page. The online version can take a few minutes to show new changes.

## Option 3: use Git (for developers)

If you already work with Git, clone the repository:

```bash
git clone https://github.com/a4ds5t/start.soholocal.git
```

Then `npm install` and `npm run dev` (Wrangler). The app is at `/app`. To get the latest changes later, run `git pull` inside the folder.
