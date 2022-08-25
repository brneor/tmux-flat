# Tmux Flat Theme

[![TPM](https://img.shields.io/badge/tpm--support-true-blue)](https://github.com/tmux-plugins/tpm)
<!-- [![Awesome](https://img.shields.io/badge/Awesome-tmux-d07cd0?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABVklEQVRIS+3VvWpVURDF8d9CRAJapBAfwWCt+FEJthIUUcEm2NgIYiOxsrCwULCwktjYKSgYLfQF1JjCNvoMNhYRCwOO7HAiVw055yoBizvN3nBmrf8+M7PZsc2RbfY3AfRWeNMSVdUlHEzS1t6oqvt4n+TB78l/AKpqHrdwLcndXndU1WXcw50k10c1PwFV1fa3cQVzSR4PMd/IqaoLeIj2N1eTfG/f1gFVtQMLOI+zSV6NYz4COYFneIGLSdZSVbvwCMdxMsnbvzEfgRzCSyzjXAO8xlHcxMq/mI9oD+AGlhqgxjD93OVOD9TUuICdXd++/VeAVewecKKv2NPlfcHUAM1qK9FTnBmQvJjkdDfWzzE7QPOkAfZiEce2ECzhVJJPHWAfGuTwFpo365pO0NYjmEFr5Eas4SPeJfll2rqb38Z7/yaaD+0eNM3kPejt86REvSX6AamgdXkgoxLxAAAAAElFTkSuQmCC)](https://github.com/rothgar/awesome-tmux) -->
<!-- [![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://wfxr.mit-license.org/2017) -->

`This is a work in progress`

A flat tmux theme based on [tmux-power](https://github.com/wfxr/tmux-power) and inspired by [kanagawa](https://github.com/rebelot/kanagawa.nvim) colors.

### 📥 Installation

**Install manually**

Clone the repo somewhere and source it in `.tmux.conf`:

```tmux
run-shell "/path/to/tmux-flat.tmux"
```

*NOTE: Options should be set before sourcing.*

**Install using [TPM](https://github.com/tmux-plugins/tpm)**

```tmux
set -g @plugin 'brneor/tmux-flat'
```

### ⚙  Customizing

You can change the date and time formats using strftime:

```tmux
set -g @tmux_flat_date_format '%F'
set -g @tmux_flat_time_format '%T'
```

You can also customize the icons:

```tmux
set -g @tmux_flat_date_icon ' ' # set it to a blank will disable the icon
set -g @tmux_flat_time_icon '🕘' # emoji can be used if your terminal supports
set -g @tmux_flat_user_icon 'U'
set -g @tmux_flat_session_icon 'S'
set -g @tmux_flat_upload_speed_icon '↑'
set -g @tmux_flat_download_speed_icon '↓'
set -g @tmux_flat_left_arrow_icon '<'
set -g @tmux_flat_right_arrow_icon '>'
```
*The default icons use glyphs from [nerd-fonts](https://github.com/ryanoasis/nerd-fonts).*

### 📦 Plugin support

**[tmux-net-speed](https://github.com/wfxr/tmux-net-speed)**

```tmux
set -g @tmux_flat_show_upload_speed true
set -g @tmux_flat_show_download_speed true
```

**[tmux-prefix-highlight](https://github.com/tmux-plugins/tmux-prefix-highlight)**

```tmux
# 'L' for left only, 'R' for right only and 'LR' for both
set -g @tmux_flat_prefix_highlight_pos 'LR'
```

**[tmux-web-reachable](https://github.com/wfxr/tmux-web-reachable)**

```tmux
set -g @tmux_flat_show_web_reachable true
```

### 🔗 Other plugins

You might also find these useful:

- [tmux-fzf-url](https://github.com/wfxr/tmux-fzf-url)
- [tmux-net-speed](https://github.com/wfxr/tmux-net-speed)
- [tmux-web-reachable](https://github.com/wfxr/tmux-web-reachable)

### 📃 License

[MIT](https://wfxr.mit-license.org/2017) (c) Wenxuan Zhang
