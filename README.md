# Night Owl Light theme

## Adding the themes

1. Create a theme folder in bat's configuration directory by running:

```bash
mkdir -p "$(bat --config-dir)/themes"
```

2. Copy the theme files from this repository:

```bash
wget -P "$(bat --config-dir)/themes" https://github.com/catppuccin/bat/raw/main/Night%20Owl%20Light.tmTheme
```

3. Rebuild bat's cache:

```bash
bat cache --build
```

4. Run `bat --list-themes`, and check if the themes are present in the list.

## Usage

There are two ways to get `bat` to default to Night Owl Light:

### Configuration file

Edit your configuration file, located at `bat --config-file` (usually `~/.config/bat/config`):

```
--theme="Night Owl Light"
```

### Environment variable

You can alternatively use the `BAT_THEME` environment variable. Export the environment variable inside your shell's configuration file: `BAT_THEME="Night Owl Light"`.

The method to export the variable depends on your shell.

### Extra: using bat as a manpager

See https://github.com/sharkdp/bat#man for instructions on how to use `bat` for your `man` output.
