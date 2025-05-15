# 📁 tree.py

`tree.py` is a lightweight Python script that generates a clean directory tree representation of your folder structure and saves it to a `structure.txt` file. It automatically ignores common temporary and environment files like `.pyc`, `.git`, `__pycache__`, `node_modules`, etc.

---

## ✨ Features

- Outputs a visual tree structure to `structure.txt`
- Ignores clutter like:
  - Virtual environments (`.venv`, `.mypy_cache`, etc.)
  - Temporary/system files (`.DS_Store`, `.log`, `.tmp`, etc.)
  - Build and IDE folders (`__pycache__`, `.vscode`, `.idea`, etc.)
- Works recursively for all subfolders
- Simple CLI usage

---

## 📦 Installation

No installation required. Just make sure you have Python 3 installed.

---

## 🚀 Usage

```bash
python tree.py [folder_path]
````

### Example

To scan the current directory:

```bash
python tree.py
```

To scan a specific folder:

```bash
python tree.py /path/to/your/folder
```

This will create a file named `structure.txt` in the same directory where the script is run, containing the folder tree.

---

## 🧼 Ignored Items

By default, the script ignores:

### Folders

* `.git`
* `.venv`
* `__pycache__`
* `node_modules`
* `.vscode`, `.idea`, `.mypy_cache`

### Files

* `.DS_Store`
* `Thumbs.db`

### Extensions

* `.pyc`
* `.pyo`
* `.log`
* `.tmp`
* `.bak`

---

## 📄 Output Format

```
your-folder/
├── file1.txt
├── subfolder1/
│   └── file2.md
└── subfolder2/
    ├── file3.py
    └── nested/
        └── file4.txt
```

---

## 🛠️ Customization

Feel free to modify the `IGNORED_*` sets in the script if you want to adjust which files or folders should be skipped.

---
## 🤖 Author Note
This script was created entirely through prompt engineering using generative AI (ChatGPT).
The author's role was to guide and instruct the AI step-by-step to produce a useful and clean solution.

## 📜 License

MIT License – free to use and modify.

