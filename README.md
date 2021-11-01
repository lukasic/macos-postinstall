# macos-postinstall

## Apps

- Eset Cyber Security, https://www.eset.com/sk/internetova-ochrana-domacnosti/cyber-security/download/
- VLC, https://videolan.org
- Firefox, https://www.mozilla.org/sk/firefox/new/
- Spotify, https://www.spotify.com/sk-en/download/mac/
- iTerm2, https://iterm2.com/
- Wireguard, https://www.wireguard.com/install/
- MacDown, https://macdown.uranusjr.com/
- JDownloader, https://jdownloader.org/download/index
- [DEV] Sublime Text, https://www.sublimetext.com/
- [DEV] Sequel Pro, https://sequelpro.com/test-builds
- [MBP] Turbo Boost Switcher, http://tbswitcher.rugarciap.com/
- [MBP] Google Chrome


Crypto Apps:
- Trezor, https://trezor.io/
- My Monero, https://mymonero.com/

App Store:

- System Monitor, https://apps.apple.com/cz/app/system-monitor/id423368786?mt=12

Future Candidates:

- AltStore, https://altstore.io/

## Brew

https://brew.sh/

Tools: axel duti

## Default apps

```bash
brew install duti
```

```bash
for ext in avi mkv mpeg mpg mp4 mp3 aac mov; do
  echo "org.videolan.vlc $ext all" | duti
done
```

```bash
for ext in py php c cpp h hpp go json xml sh conf cfg yml yaml ini; do
  echo "com.sublimetext.4 $ext all" | duti
done
```

## Tweaks

**Allow apps from everywhere:**

```bash
sudo spctl --master-enable
```
