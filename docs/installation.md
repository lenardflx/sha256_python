## Installation Guide

#### From PyPI (recommended)

```bash
pip install sha256py
```

#### From GitHub

```bash
git clone https://github.com/lenardflx/sha256_python.git
cd sha256_python
pip install -e .
```

#### Without installing (No access to the `sha256py` command)


```bash
git clone https://github.com/lenardflx/sha256_python.git
cd sha256_python
python -m sha256py.cli "hello"
```

---

### Enabling the `sha256py` command globally

Do this if `sha256py` isnt installed to your system's PATH:

#### PowerShell

```powershell
$env:Path += ";$env:USERPROFILE\\AppData\\Roaming\\Python\\Scripts"
```

or add path permanently in Environment Variables > PATH

#### Linux/macOS

Add to your `~/.bashrc`, `~/.zshrc`, or different shell config:

```bash
export PATH="$HOME/.local/bin:$PATH"
```

Then reload your shell:

```bash
source ~/.bashrc  # or source ~/.zshrc
```

Run to verify that it works globally:

```bash
sha256py --help
```