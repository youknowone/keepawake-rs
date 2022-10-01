# keepawake-rs
Keep your computer awake. Like [`caffeinate`], [`systemd-inhibit`]/[`gnome-session-inhibit`], or [PowerToys Awake], but cross-platform and written in [Rust].

[`caffeinate`]: https://ss64.com/osx/caffeinate.html
[`systemd-inhibit`]: https://www.freedesktop.org/software/systemd/man/systemd-inhibit.html
[`gnome-session-inhibit`]: https://manpages.ubuntu.com/manpages/jammy/man1/gnome-session-inhibit.1.html
[PowerToys Awake]: https://learn.microsoft.com/en-us/windows/powertoys/awake
[Rust]: https://www.rust-lang.org/

## Usage
```
Keep your computer awake

Usage: keepawake.exe [OPTIONS] [COMMAND]...

Arguments:
  [COMMAND]...  Run the command and wait for it to exit, keeping the computer awake while it runs

Options:
  -d, --display              Keep display on
  -i, --idle                 Keep system from idle sleeping
  -s, --sleep                Keep system from sleeping (Functionality and conditions for this to work vary by OS)
      --completions <SHELL>  Generate shell completions [possible values: bash, elvish, fish, powershell, zsh]
  -h, --help                 Print help information
  -V, --version              Print version information
```

## Installation

### Cargo
```sh
cargo install keepawake
```

### Binaries
Will be made available later.

## Notes
Preventing the computer from explicitly sleeping, and/or by closing the lid, is often restricted in various ways by the OS, e.g. Only on AC power, not in any PC running Windows with [Modern Standby](https://learn.microsoft.com/en-us/windows-hardware/design/device-experiences/modern-standby).

## License
MIT License.
