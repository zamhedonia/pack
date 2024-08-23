## paxs

`paxs` is a simple and convenient Bash script for searching packages across three different package managers: Yay (AUR), Flatpak, and Snap.

 It streamlines the process of finding packages across multiple package formats with a single command.

### Installation

1. Download the script:
   ```bash
   git clone https://github.com/zamhedonia/paxs.git
   ```
   
2. Open the directory:
   ```bash
   cd ~/paxs
   ```
   
3. Make it executable:
   ```bash
   chmod +x paxs
   ```

4. Move the script to a directory in your `$PATH` (e.g., `/usr/local/bin`):
   ```bash
   sudo mv paxs /usr/local/bin/paxs
   ```

5. Now you can use `paxs` from anywhere in your terminal!

### Usage

To search for a package, simply type `paxs <search_term>`.

For example:
```bash
paxs firefox
```

This command will search for the package "firefox" in:
- Yay (Arch Repository and Arch User Repository)
- Flatpak
- Snap

You'll receive the results from each package manager, one after the other.

### Example Output

```bash
paxs firefox
```
```bash
Searching for 'firefox' in Yay, Flatpak, and Snap...

Yay search:
firefox 89.0-1 [installed] (mozilla)

Flatpak search:
firefox stable flathub org.mozilla.firefox

Snap search:
firefox (v89.0) mozilla - Firefox Web Browser
```

### Help

For help or usage instructions, use the `-h` option:
```bash
paxs -h
```


--------

```bash
paxs moo
```
