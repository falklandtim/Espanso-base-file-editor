# Espanso Editor

A visual editor for managing your [Espanso](https://espanso.org/) YAML configuration files. No installation required - just download and open in your browser!

DISCLOSURE: This html file and README file was made with Claude AI. I am not a coder 😂

![Espanso Editor](https://img.shields.io/badge/espanso-editor-blue)
![No Dependencies](https://img.shields.io/badge/dependencies-none-green)
![License](https://img.shields.io/badge/license-MIT-blue)

## ✨ Features

- 📤 **Upload & Merge** - Load your existing `base.yml` and merge additional YAML files
- ✏️ **Visual Editor** - Add, edit, and delete matches with an intuitive interface
- 🔍 **Preview** - See exactly how your text will appear when expanded
- ⚠️ **Duplicate Detection** - Automatically find and remove duplicate triggers
- 🧹 **Auto-Cleanup** - Converts escaped characters (`\n`, `\t`, etc.) to proper formatting
- 💾 **Download** - Export your cleaned YAML file ready for Espanso
- 🌐 **Works Offline** - No internet connection needed after initial load
- 🚫 **No Installation** - Pure HTML/CSS/JavaScript - just open and use!

## 🚀 Quick Start

### Option 1: Download and Use
1. Download `espanso_standalone.html` from this repository
2. Double-click the file to open in your browser
3. Click "Upload Base YAML" and select your Espanso `base.yml` file
4. Edit, add, or remove matches as needed
5. Click "Download YAML" to save your updated file

### Option 2: Use Online
Simply open the file in any modern browser (Chrome, Firefox, Safari, Edge).

## 📍 Where is my Espanso config?

Your Espanso configuration file is typically located at:

**macOS:**
```
~/Library/Application Support/espanso/match/base.yml
```

**Linux:**
```
~/.config/espanso/match/base.yml
```

**Windows:**
```
%APPDATA%\espanso\match\base.yml
```

## 🎯 Usage

### Upload Your Base File
Click "Upload Base YAML" to load your existing Espanso configuration. The editor will automatically:
- Parse your YAML file
- Convert escaped characters to proper formatting
- Display all your matches in a clean interface

### Merge Additional Files
Already have a base file loaded? Click "Merge Another YAML" to add matches from another file. The editor will:
- Skip duplicates automatically
- Show you which triggers were added
- Keep your existing matches safe

### Add New Matches
Click "Add New" to create a new text expansion shortcut:
- **Trigger**: The shortcut you'll type (e.g., `;em` or `:email`)
- **Replace**: The text that will appear (supports multi-line text)

### Handle Duplicates
If you have duplicate triggers, the editor will alert you:
- **Review & Remove** - See all duplicates side-by-side and choose which to keep
- **Auto-Remove** - Automatically keep the first occurrence of each duplicate

### Preview Your Matches
Click the 👁️ icon next to any match to see exactly how the replacement text will appear, including proper line breaks and formatting.

### Download Your Updated File
Click "Download YAML" to save your cleaned configuration file. Replace your old `base.yml` with this new one and restart Espanso.

## 🔧 Common Use Cases

### Cleaning Up Messy Exports
Got a YAML file with escaped characters like `\n` everywhere? Just upload it and the editor automatically converts them to proper line breaks.

**Before:**
```yaml
replace: "Line 1\nLine 2\nLine 3"
```

**After upload, the editor shows:**
```
Line 1
Line 2
Line 3
```

### Merging Multiple Files
Combining shortcuts from different sources? Upload your base file, then merge others one by one. The editor prevents duplicates automatically.

### Finding and Fixing Duplicates
Not sure if you have duplicate triggers? The editor detects them instantly and helps you clean them up with visual comparison.

## 🛠️ Technical Details

- **No Dependencies**: Pure HTML, CSS, and vanilla JavaScript
- **Privacy First**: Everything runs locally in your browser - no data is sent anywhere
- **Lightweight**: Single ~50KB HTML file
- **Compatible**: Works in all modern browsers

## 📝 Example Workflow

1. **Backup your current config** (always a good idea!)
   ```bash
   cp ~/.config/espanso/match/base.yml ~/.config/espanso/match/base.yml.backup
   ```

2. **Open the editor** in your browser

3. **Upload your base.yml** file

4. **Make your changes** (add, edit, remove, clean up duplicates)

5. **Download the updated file**

6. **Replace your old config**
   ```bash
   cp ~/Downloads/base.yml ~/.config/espanso/match/base.yml
   ```

7. **Restart Espanso**
   ```bash
   espanso restart
   ```

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📄 License

MIT License - feel free to use, modify, and distribute!

## 🙏 Credits

Built for the [Espanso](https://espanso.org/) community - the amazing open-source text expander.

## 💬 Support

Having issues? Found a bug? [Open an issue](../../issues) on GitHub!

---

**Made with ❤️ for the Espanso community**

*Save time, type less, do more!*
