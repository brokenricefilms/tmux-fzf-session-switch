# TMUX FZF Session Switch (fork)

**↓↓Table of Contents↓↓**

- [TMUX FZF Session Switch (fork)](#tmux-fzf-session-switch-fork)
  - [Customization from me](#customization-from-me)
  - [Two way, You want customize key binding](#two-way-you-want-customize-key-binding)
  - [Purpose](#purpose)
  - [Install](#install)
  - [Functionality](#functionality)
  - [Requirements](#requirements)

---

![Demo](./img/20211130134835.png)

## Customization from me

- Work with session name have `space` character. e.g. "Thuan Pham is handsome"
- Don't confirm `y` to create new session, I just lazy press 2 time `Enter` to create new session.
- Pop-up windown instead of new window (required tmux >= 3.2)

## Two way, You want customize key binding

1. You can folk this project and edit this line `default_key_bindings_goto="C-f"` in `main.tmux`, you change `set -g @plugin '{{your github username}}/tmux-fzf-session-switch' in your tmux config
2. You can create pull request, "feature custom keybinding" is good too 😁 cuz I'm noob and lazy to make this feature.

## Purpose

If you're like me and you tend to have a lot of sessions to organize your
thoughts then this is the plugin for you. With this plugin you can search
through your sessions with fzf.

## Install

- Install this <https://github.com/tmux-plugins/tpm>
- Put `set -g @plugin 'thuanpham2311/tmux-fzf-session-switch' into your tmux config
- Use tpm install plugin. Default you can press `prefix + I` (`I` is `shirt + i` = I)
- Finally. `Hold ctrl -> press a -> press f`
  > my prefix is `ctrl + a`

## Functionality

- `Prefix + `: Open up fzf in a new tab. (e.g. prefix = ctrl + a. Hold ctrl -> press a -> press f -> done)
- If you type a name that doesn't exist, you will be prompted to create it.

## Requirements

- [fzf](https://github.com/junegunn/fzf)
- rg (recommended but not required)
