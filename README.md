# Omarchy Vazirmatn Font

This package provides the Vazirmatn Persian font and fontconfig rules for Omarchy/Arch Linux.
- Installs variable TTF font into `/usr/share/fonts/TTF/`
- Provides a fontconfig rule to prefer Vazirmatn for Persian (fa) text
- Automatically activates the font via symlink in `/etc/fonts/conf.d/`

## Installation

```bash
# Build and install locally
makepkg -si

