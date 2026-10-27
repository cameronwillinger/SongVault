# SongVault Mobile — iPhone setup (one page)

## Install
1. On your iPhone, open **Safari** (it must be Safari, not Chrome) and go to **https://cameronwillinger.github.io/SongVault/**.
2. Tap **Share** (square with arrow) ▸ **Add to Home Screen** ▸ **Add**.
3. Open **SongVault** from the Home Screen. Tap **Allow** for microphone if you want to record. It works offline after the first load.
4. In the app: **Sync** tab ▸ **Request persistent storage** so iOS is less likely to clear it.

## First sync (desktop ▸ phone)
1. On the PC, open SongVault, then Sync/Export ▸ **Export Sync File** (a `….songvault.zip`).
2. Move it to the phone: **AirDrop**, iCloud Drive, OneDrive, or email it to yourself.
3. On the phone: **Sync** ▸ **Choose sync file…** ▸ pick the zip. Check the preview (X added, Y updated, Z conflicts) ▸ **Apply**.

## Syncing back (phone ▸ desktop)
1. Phone: **Sync** ▸ **Build Sync File** ▸ **Share / Save to Files…** (AirDrop to the Mac/PC, or Save to Files / iCloud Drive).
2. Desktop: **Import Sync File**, pick the zip, review the preview, **Apply merge**.
3. Repeat in either direction any time. Importing the same file twice changes nothing.
4. Optional: put Grok answers in `grok-inbox/*.json` (`songId`, `section`, `text`, optional `links`) in a folder on your computer and use **Import Grok Inbox JSON…** (phone: Sync tab; desktop: Sync menu or the Grok tool).

## Limits to know
- **Sync is manual.** There is no cloud and no background sync. Export after a writing session.
- **iOS can clear website data** if storage is low, or after about 7 days unused when the app is not on the Home Screen. Export a Sync File regularly. The Sync tab shows "Last backed up".
- Big videos make a huge sync file. Turn **Include media** off and AirDrop the video files separately.
- Mic/camera need the HTTPS link. Voice memos are saved as .m4a on iPhone.
- Removing artwork on the phone may not remove it on the desktop on the next merge (the merge never deletes).
- The phone uses the generic Grok co-writer rules. Edit them under the Grok tool's template, or paste your own.
- Grok prompt boxes copy a prompt for you to paste into your Grok chat, then paste the answer back. Nothing is sent automatically.
