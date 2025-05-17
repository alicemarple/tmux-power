# Tmux Theme

Yet another theme for tmux.

![screenshot](https://raw.githubusercontent.com/wfxr/i/master/tmux-power-custom.png)

### 📥 Installation

**Install manually**

Clone the repo somewhere and source it in `.tmux.conf`:

```tmux
run-shell "/path/to/tmux-power.tmux"
```

_NOTE: Options should be set before sourcing._

**Install using [TPM](https://github.com/tmux-plugins/tpm)**

```tmux
set -g @plugin 'alicemarple/tmux-power'
```

### 🎨 Themes

#### Gold (default)

```bash
set -g @tmux_power_theme 'gold'
```

![screenshot](https://raw.githubusercontent.com/wfxr/i/master/tmux-power-gold.png)

#### Everforest

```bash
set -g @tmux_power_theme 'everforest'
```

![screenshot](https://raw.githubusercontent.com/wfxr/i/master/tmux-power-everforest.png)

#### Moon

```bash
set -g @tmux_power_theme 'moon'
```

![screenshot](https://raw.githubusercontent.com/wfxr/i/master/tmux-power-moon.png)

#### Coral

```bash
set -g @tmux_power_theme 'coral'
```

![screenshot](https://raw.githubusercontent.com/wfxr/i/master/tmux-power-coral.png)

#### Snow

```bash
set -g @tmux_power_theme 'snow'
```

#### Forest

```bash
set -g @tmux_power_theme 'forest'
```

Violet

```bash
set -g @tmux_power_theme 'violet'
```

#### Redwine

```bash
set -g @tmux_power_theme 'redwine'
```

### ⚙ Customizing

You can define your favourite colors if you don't like any of above.

```tmux
# You can set it to a true color in '#RRGGBB' format
set -g @tmux_power_theme '#483D8B' # dark slate blue

# Or you can set it to 'colorX' which honors your terminal colorscheme
set -g @tmux_power_theme 'colour3'

# The following colors are used as gradient colors
set -g @tmux_power_g0 "#262626"
set -g @tmux_power_g1 "#303030"
set -g @tmux_power_g2 "#3a3a3a"
set -g @tmux_power_g3 "#444444"
set -g @tmux_power_g4 "#626262"
```

You can change the date and time formats using strftime:

```tmux
set -g @tmux_power_date_format '%F'
set -g @tmux_power_time_format '%T'
```

You can also customize the icons. As an example,
the following configurations can generate the theme shown in the first screenshot:

```bash
set -g @plugin 'wfxr/tmux-power'
set -g @plugin 'wfxr/tmux-net-speed'
set -g @tmux_power_theme 'everforest'
set -g @tmux_power_date_icon           ' '
set -g @tmux_power_time_icon           ' '
set -g @tmux_power_user_icon           ' '
set -g @tmux_power_session_icon        ' '
set -g @tmux_power_right_arrow_icon    ''
set -g @tmux_power_left_arrow_icon     ''
set -g @tmux_power_upload_speed_icon   '󰕒'
set -g @tmux_power_download_speed_icon '󰇚'
```

The following components can be toggled on or off:

```tmux
set -g @tmux_power_show_user    true
set -g @tmux_power_show_host    true
set -g @tmux_power_show_session true
```

_The default icons use glyphs from [nerd-fonts](https://github.com/ryanoasis/nerd-fonts)._

### 📦 Plugin support

**[tmux-net-speed](https://github.com/wfxr/tmux-net-speed)**

```tmux
set -g @tmux_power_show_upload_speed   true
set -g @tmux_power_show_download_speed true
```

**[tmux-prefix-highlight](https://github.com/tmux-plugins/tmux-prefix-highlight)**

```tmux
# 'L' for left only, 'R' for right only and 'LR' for both
set -g @tmux_power_prefix_highlight_pos 'LR'
```

**[tmux-web-reachable](https://github.com/wfxr/tmux-web-reachable)**

```tmux
set -g @tmux_power_show_web_reachable true
```

### 🔗 Credits

This project is based on the excellent work of **@wfxr** in their repository : https://github.com/wfxr/tmux-power.

I have made the following modifications:

- Prefix key visual indicator

### 🔗 Other plugins

You might also find these useful:

- [tmux-fzf-url](https://github.com/wfxr/tmux-fzf-url)
- [tmux-net-speed](https://github.com/wfxr/tmux-net-speed)
- [tmux-web-reachable](https://github.com/wfxr/tmux-web-reachable)
