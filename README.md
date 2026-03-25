# Dotfiles

Personal configuration files managed with [GNU Stow](https://www.gnu.org/software/stow/).

## Packages

| Package | Description |
|---------|-------------|
| `bin` | Shell scripts and utilities |
| `git` | Git configuration |
| `myenv` | Shell environment, aliases, fzf functions |
| `starship` | Starship prompt |
| `systemd` | User systemd services (rclone mounts) |
| `vim` | Vim configuration |
| `vscode` | VSCode settings and keybindings |
| `zsh` | Zsh configuration |

## Usage

```bash
# Install a package (symlinks into ~/)
stow <package>

# Remove a package
stow -D <package>
```

## Notes

- **systemd user services** require `loginctl enable-linger` to start at boot without login.
- Per-instance env files for rclone mounts live at `~/.config/rclone/mounts/` (not tracked by git).
