# tm:rw Brand Asset Manager — Releases

Public release binaries for the (private) **tm:rw Brand Asset Manager** app.
Built and published automatically by GitHub Actions. The desktop app's built-in
auto-updater reads `latest.json` from the newest release here. Source is private.

## Download

Grab the newest build from the [latest release](../../releases/latest):

- **macOS (Apple Silicon)** — `..._aarch64.dmg`
- **Windows** — `..._x64-setup.exe`

You only download manually for the **first install**. After that the app
auto-updates itself.

## Mac says the app "is damaged and can't be opened"?

It isn't damaged. The Mac build isn't yet notarised by Apple, so macOS
quarantines the download and shows that message. Two ways to fix it:

- **Easy:** download **`Fix-tmrw-Mac.zip`** from the [latest release](../../releases/latest),
  unzip it, and double-click **`Fix-tmrw-Mac.command`**. It clears the flag and
  opens the app. (First run: if macOS blocks the script too, right-click it →
  **Open** → **Open**.)
- **Manual:** drag the app into Applications, then run this in Terminal:
  ```bash
  xattr -cr "/Applications/tmrw Brand Asset Manager.app"
  ```

This step goes away once the app is signed + notarised.
