<h2 align="center">🗼 Tokyo Night SDDM 🗼</h2>

<p align=center>
A Tokyo Night theme for the <a href="https://github.com/sddm/sddm">SDDM Login Manager</a>
</p>

<h2 align=center>Preview</h2>
<center>
<img src="./Previews/1.png" alt="preview-1">
<details>
<summary align=center>More Previews</summary>
<img src="./Previews/2.png" alt="preview-2">
<img src="./Previews/3.png" alt="preview-4">
<img src="./Previews/4.png" alt="preview-3">
</details>
</center>

## Install
### From sources
> _Assumes that you've installed and configured SDDM correctly_ (if not [read more](https://wiki.archlinux.org/title/SDDM))

>  Please make sure you have the following dependencies installed:
>  `qt5-quickcontrols2`, `qt5-graphicaleffects`, `qt5-svg` 

1. Open terminal, and clone the repository with:

   ```sh
   git clone https://github.com/rototrash/tokyo-night-sddm.git ~/tokyo-night-sddm
   ```

2. Them move it as follows:

   ```sh
   sudo mv ~/tokyo-night-sddm /usr/share/sddm/themes/
   ```

### Arch Linux
This theme is available on the [AUR](https://aur.archlinux.org/packages/sddm-theme-tokyo-night), you can install it with `makepkg` or using an AUR helper.

```sh
git clone https://aur.archlinux.org/sddm-theme-tokyo-night.git
cd sddm-theme-tokyo-night
makepkg -Ccsi
```

## Configure

Edit the `/etc/sddm.conf` (with any text editor with **raised** privileges), so that it looks like this:

```sh
sudo nano /etc/sddm.conf  # use any text editor with raised privileges
---
[Theme]
Current=tokyo-night-sddm
   ```

### Language and time format

- You can also change the time format.
- To change the default wallpaper put desired image in the `tokyo-night-sddm/Backgrounds/` folder and add the name of the image followed by its extension (`.jpg` or `.png`) in `theme.conf` file.
- You can also customize it further if you wish in the `theme.conf`
(blur, form position, etc).
## Credits

- Based on the theme [`Sugar Dark for SDDM`](https://github.com/MarianArlt/sddm-sugar-dark) by [**MarianArlt**](https://github.com/MarianArlt).
- AUR Package by [**julian-poidevin**](https://github.com/julian-poidevin)

## License

[GNU Lesser General Public License v3.0](LICENSE)
