# dotfiles-gruvbox
a dotfiled rice with a vertical bar (+ a togglebale second vertical bar). tested for functionality and reproduceability on Arch Linux (kernel 6.10.5)

## Previews
![2024-08-17T21:05:44,704559941+03:00](https://github.com/user-attachments/assets/9eb36c33-3bb0-4a2f-a2df-c2292e1946b6)
![2024-08-17T21:07:29,729463961+03:00](https://github.com/user-attachments/assets/fbb00480-a897-4864-b65b-53b34f189e0f)
![2024-08-17T22:09:37,672697948+03:00](https://github.com/user-attachments/assets/e0685cc6-65ce-4946-9f09-f61f72c0ef77)

## Packages/Dependencies Used
### swaywm and co. (major UI elements)
- wm: [`swayfx`]([https://github.com/swaywm/sway](https://github.com/WillPower3309/swayfx)) (forked from [`sway`](https://github.com/swaywm/sway) for rounded corners, shadows, and a few more enhancements)
    
> [!NOTE]
> The config files for sway depend on GNOME's GTK4.0 theming for `libadwaita` apps (i'm a GNOME departee!), as well as for user authentication within `nautilus` (via `polkit`). You may want to remove/rewrite those portions accordingly).
- main bottom bar: [`waybar`](https://github.com/Alexays/Waybar)
- lockscreen: [`swaylock`](https://github.com/swaywm/swaylock) (not shown, plain :) )
- notification daemon: [`dunst`](https://github.com/dunst-project/dunst)
- app launcher and logout options: [`rofi`](https://github.com/davatorium/rofi) with themes based on configs from [adi1090x's repo](https://github.com/adi1090x/rofi?tab=readme-ov-file)

### extra dependencies required (check after your sway config copy)
- sway: `brightnessctl` `playerctl` `pamixer` `wob` (audio/brightness keybindings and progress bar), `polkit`/`polkit-gnome-authentication` (user authentication for `nautilus`), `grimshot` (for screenshots), `wf-recorder` (for screen recordings, grapped from [ugursogukpinar's gist](https://gist.github.com/ugursogukpinar/f390d9f4c829fb1b05fc74a12dd482bb)), `swayidle` (for idle settings), `swaybg` (for backgrounds, issues with this dependency missing reported on Arch), scripts for scheduling low battery and charging alerts (from [Eric Murphy's dotfiles' scripts](https://github.com/ericmurphyxyz/dotfiles/tree/master/.local/bin))
- waybar: `playerctl` (for MPRIS media module)

### terminal stuff
- terminal: [`kitty`](https://github.com/kovidgoyal/kitty)
- shell: `bash` with [`ble.sh`](https://github.com/akinomyoga/ble.sh) modified with [`fish` like autocomplete](https://harduex.com/blog/fish-like-autosuggestions-in-bash-shell/)
- text editor: [`nvim`](https://github.com/neovim/neovim) with [LazyVim](https://github.com/LazyVim/LazyVim)
- fetch: [`fastfetch`](https://github.com/fastfetch-cli/fastfetch)

### theming stuff
- theme: [tinted-theming's base16](https://github.com/tinted-theming/home) [gruvbox-dark-medium](https://tinted-theming.github.io/base16-gallery/)... here's [more info on morhetz's Gruvbox theme](https://github.com/morhetz/gruvbox)... for libadwaita apps (GTK4.0), check [Fausto-Korpsvart's repo](https://github.com/Fausto-Korpsvart/Gruvbox-GTK-Theme)
- browser: Firefox CSS mods from [csshacks](https://github.com/MrOtherGuy/firefox-csshacks)
- wallpaper: custom made [relative link](.config/sway/nadekodrowndark.png)
- spotify: [`spicetify-cli`](https://spicetify.app/) with [modified](.config/spicetify/Themes/text/) [text theme](https://github.com/spicetify/spicetify-themes/tree/master/text)
- fonts: [Jetbrains Mono](https://github.com/JetBrains/JetBrainsMono)
- cursor: [Bibata-Modern-Classic](https://www.bibata.live/) (not shown in screenshots)
