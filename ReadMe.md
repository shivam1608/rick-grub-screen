# Rick GRUB Screen Theme

A custom GRUB2 bootloader theme featuring Rick and Morty styling with terminal fonts and custom icons.

## Installation

```
git clone https://github.com/shivam1608/rick-grub-screen.git
```

### Fedora

1. **Install GRUB2 packages:**
   ```bash
   sudo dnf install grub2-tools
   ```

2. **Copy the theme to GRUB themes directory:**
   ```bash
   sudo cp -r ~/rick-grub-screen /usr/share/grub/theme/
   ```

3. **Update GRUB configuration:**
   Edit `/etc/default/grub` and:
   - Add/modify the following line:
     ```
     GRUB_THEME="/usr/share/grub/theme/rick-grub-screen/theme.txt"
     ```
   - **Comment out the `GRUB_TERMINAL_INPUT` line** (if present):
     ```
     # GRUB_TERMINAL_INPUT="console"
     ```

4. **Regenerate GRUB configuration:**
   ```bash
   sudo grub2-mkconfig -o /boot/grub2/grub.cfg
   ```

5. **Reboot to apply the theme:**
   ```bash
   sudo reboot
   ```

### Debian-based Systems (Ubuntu, Linux Mint, etc.)

1. **Install GRUB2 packages:**
   ```bash
   sudo apt-get install grub2 grub-customizer
   ```

2. **Copy the theme to GRUB themes directory:**
   ```bash
   sudo cp -r ~/rick-grub-screen /boot/grub/themes/
   ```

3. **Update GRUB configuration:**
   Edit `/etc/default/grub` and add/modify the following line:
   ```
   GRUB_THEME="/boot/grub/themes/rick-grub-screen/theme.txt"
   ```

4. **Regenerate GRUB configuration:**
   ```bash
   sudo grub-mkconfig -o /boot/grub/grub.cfg
   ```

5. **Reboot to apply the theme:**
   ```bash
   sudo reboot
   ```

## Files Included

- `theme.txt` - Main theme configuration
- `terminus-*.pf2` - Terminus font files in various sizes
- `unifont-*.pf2` - Unifont files for extended character support
- `icons/` - Directory containing custom icons and graphics

## Credits

- **Icons**: [icons8](https://icons8.com) - For providing the custom icons used in this theme
- **Background**: [wafelman](https://github.com/wafelman) - For the original background design

## License

Please refer to the original sources for license information regarding the icons and background used in this theme.

## Open Source Project

Author : Shivzee
<br />
[Buy me a coffee](https://buymeacoffee.com/shivzee)

