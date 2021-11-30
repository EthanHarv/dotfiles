# A Simple BSPWM Setup

## Installation (assumes Ubuntu 21.10 or similar)

Install the required packages:

```bash
sudo apt update && sudo apt upgrade
sudo apt install bspwm kitty rofi picom polybar nitrogen
```

Copy all `.config` folders into `~/.config/`

Add bspwm to `.xinit` (sometimes not needed, but issues can occur if you don't)

```bash
nano ~/.xinit
```

```bash
#!/bin/bash
exec bspwm
```

Install RobotoMono and Iosevka from [here](https://github.com/ryanoasis/nerd-fonts/releases/latest) by unzipping and copying to `/usr/local/share/fonts`, and do `fc-cache -f -v` after (or restart).
