# dotfiles-gruvbox
a dotfiled rice with a vertical bar (+ a togglebale second vertical bar)

## Previews
![2024-08-03T01:57:27,151835401+03:00](https://github.com/user-attachments/assets/15a0654f-3395-49ea-9e7e-506e33e2e864)
![2024-08-03T01:57:36,070711581+03:00](https://github.com/user-attachments/assets/4c75aeaf-f0f9-4365-9fa9-ebda9a5bc614)
![2024-08-03T01:58:13,437432500+03:00](https://github.com/user-attachments/assets/4978406a-5907-48ef-8ac4-1d5624458008)
![2024-08-03T02:06:15,272718247+03:00](https://github.com/user-attachments/assets/251eea48-320b-4b1f-9bfd-c34649931324)

## Packages/Dependencies Used
### swaywm and co. (major UI elements)
- wm: [`swayfx`]([https://github.com/swaywm/sway](https://github.com/WillPower3309/swayfx)) (forked from [`sway`](https://github.com/swaywm/sway) for rounded corners, shadows, and a few more enhancements)
    
> [!NOTE]
> The config files for sway depend on GNOME's GTK4.0 theming for `libadwaita` apps (i'm a GNOME departee!), as well as for user authentication within `nautilus` (via `polkit`). You may want to remove/rewrite those portions accordingly).
- main bottom bar: [`waybar`](https://github.com/Alexays/Waybar)
- lockscreen: [`swaylock`](https://github.com/swaywm/swaylock) (not shown, plain :) )
- notification daemon: [`dunst`](https://github.com/dunst-project/dunst)
- app launcher and logout options: [`rofi`](https://github.com/davatorium/rofi) with themes based on configs from [adi1090x's repo](https://github.com/adi1090x/rofi?tab=readme-ov-file).

### extra dependencies required (check after your sway config copy)
- sway: `brightnessctl` `playerctl` `pamixer` `wob` (audio/brightness keybindings and progress bar), `polkit`/`polkit-gnome-authentication` (user authentication for `nautilus`), `grimshot` (for screenshots), `wf-recorder` (for screen recordings, grapped from [ugursogukpinar's gist](https://gist.github.com/ugursogukpinar/f390d9f4c829fb1b05fc74a12dd482bb)), `swayidle` (for idle settings), `swaybg` (for backgrounds, issues with this dependency missing reported on Arch), `crontab` for scheduling low battery and charging dunst alerts (from [Eric Murphy's dotfiles' scripts](https://github.com/ericmurphyxyz/dotfiles/tree/master/.local/bin))
- waybar: `playerctl` (for MPRIS media module)

### terminal stuff
- terminal: [`kitty`](https://github.com/kovidgoyal/kitty)
- shell: `bash` with [`ble.sh`](https://github.com/akinomyoga/ble.sh) modified with [`fish` like autocomplete](https://harduex.com/blog/fish-like-autosuggestions-in-bash-shell/)
- text editor: [`nvim`](https://github.com/neovim/neovim) with [LazyVim](https://github.com/LazyVim/LazyVim)
- fetch: [`fastfetch`](https://github.com/fastfetch-cli/fastfetch) (with custom image)

### theming stuff
- theme: [tinted-theming's base16](https://github.com/tinted-theming/home) [gruvbox-dark-medium](https://tinted-theming.github.io/base16-gallery/)... here's [more info on morhetz's Gruvbox theme](https://github.com/morhetz/gruvbox)... for libadwaita apps (GTK4.0), check [Fausto-Korpsvart's repo](https://github.com/Fausto-Korpsvart/Gruvbox-GTK-Theme)
- wallpaper: [link](https://gruvbox-wallpapers.pages.dev/wallpapers/minimalistic/gruv-abstract-maze.png) (original collection from [here](https://gruvbox-wallpapers.pages.dev))
- spotify: [`spicetify-cli`](https://spicetify.app/) with modified [text theme](https://github.com/spicetify/spicetify-themes/tree/master/text)
- fonts: [Jetbrains Mono](https://github.com/JetBrains/JetBrainsMono)
- cursor: [Bibata-Modern-Classic](https://www.bibata.live/) (not shown in screenshots)
