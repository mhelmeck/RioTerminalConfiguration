# Rio Terminal Configuration

This repository contains my personal configuration for the Rio terminal emulator. Rio is a modern GPU-accelerated terminal emulator written in Rust.

## Configuration Files

The repository includes:
- `config.toml` - Contains the custom terminal's appearance and behavior settings
- `themes/` - Directory containing custom color schemes
  - Each theme is defined in its own TOML file
  - The active theme is referenced in `config.toml`

## Setup

1. Clone this repository
2. Create the Rio config directory (if it doesn't exist):
   ```bash
   mkdir -p ~/.config/rio
   ```
3. Copy or symlink the configuration:
   ```bash
   # Option 1: Copy all files
   cp -r config.toml themes ~/.config/rio/

   # Option 2: Create symlinks
   ln -s /path/to/this/repo/config.toml ~/.config/rio/config.toml
   ln -s /path/to/this/repo/themes ~/.config/rio/themes
   ```

## Themes

The `themes/` directory contains custom color schemes for Rio. To use a theme:
1. Place it in the themes directory
2. Reference it in your `config.toml`:
   ```toml
   theme = "themes/your-theme-name.toml"
   ```

## Requirements

- Rio terminal emulator
- macOS (though Rio also works on other platforms)

## Additional Resources

- [Rio Terminal GitHub Repository](https://github.com/raphamorim/rio)
- [Rio Terminal Documentation](https://raphamorim.io/rio/)

## Contributing

Feel free to fork this repository and adapt the configuration to your needs. If you have suggestions for improvements, please open an issue or submit a pull request.
