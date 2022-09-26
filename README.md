# macos-postinstall

## Apps

- Eset Cyber Security, https://www.eset.com/sk/internetova-ochrana-domacnosti/cyber-security/download/
- VLC, https://videolan.org
- Plexamp, https://plexamp.com/
- Firefox, https://www.mozilla.org/sk/firefox/new/
- Spotify, https://www.spotify.com/sk-en/download/mac/
- iTerm2, https://iterm2.com/
- Wireguard, https://www.wireguard.com/install/
- MacDown, https://macdown.uranusjr.com/
- JDownloader, https://jdownloader.org/download/index
- Syncthing, https://syncthing.net/downloads/
- [DEV] VS Code, https://code.visualstudio.com/
- [DEV] Sublime Text, https://www.sublimetext.com/
- [MBP] Turbo Boost Switcher, http://tbswitcher.rugarciap.com/
- [WORK] Google Chrome

App Store:

- [DEV] Sequel Ace
- [DEV] Snippets Lab

Crypto Apps:
- Trezor, https://trezor.io/
- My Monero, https://mymonero.com/

App Store:

- iStatistica, https://apps.apple.com/cz/app/istatistica/id1025822138?mt=12

Future Candidates:

- AltStore, https://altstore.io/

## Brew

https://brew.sh/

```
echo 'export PATH="/usr/local/sbin:$PATH"' >> ~/.zshrc
```

```
brew install axel duti mtr zsh pyenv pyenv-virtualenv kubectl kubectx
```

## Oh my ZSH

https://ohmyz.sh/#install

append to .zshrc:

```
export LC_ALL="en_US.UTF-8"
export LC_CTYPE="en_US.UTF-8"

alias newpass='pwgen -s -c -y 20 1'
alias sshr='ssh-keygen -R'
```

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
