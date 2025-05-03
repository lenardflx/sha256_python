## Usage Guide

---

### As Python Library

```python
from sha256py import Sha256
my_hash = Sha256("Hello World!")
print(my_hash.hexdigest())
```

Available methods:
- `hexdigest()`: Returns the hash as a hexadecimal string.
- `digest()`: Returns the hash as a binary string.
- `bindigest()`: Returns the raw bytes of the hash.

---

### Command Line Tool

#### Basic Syntax

```bash
sha256py [OPTIONS] [INPUT | -]
```

* `INPUT`: A string to hash (optional, use `-` to read from stdin)
* If no input is provided, the tool prompts the user

---

#### Input Options

| Option               | Description                              |
|----------------------|------------------------------------------|
| `INPUT` (positional) | A literal string to hash                 |
| `-f, --file FILE`    | Read content from the specified file     |
| `--silent`           | Prompt input securely (hides typed text) |
| `-`                  | Read from stdin                          |

Examples:

```bash
sha256py "hello world"
sha256py -f notes.txt
cat data.txt | sha256py -
sha256py --silent
```

---

#### Output Options

| Option      | Description                                 |
|-------------|---------------------------------------------|
| `--raw`     | Output the binary digest (to stdout buffer) |
| `--binary`  | Output the digest as a binary string        |
| *(default)* | Outputs the digest in hexadecimal (default) |

Examples:

```bash
sha256py "abc" > hash.txt           # hex output
sha256py "abc" --binary             # binary string
sha256py "abc" --raw > hash.bin     # raw bytes
```

---

#### Debugging & Dev Options

| Option          | Description                                                |
|-----------------|------------------------------------------------------------|
| `--time`        | Shows the duration of the process                          |
| `--log`         | Print internal state and rounds (for educational purposes) |
| `-v, --version` | Print version and exit                                     |

Examples:

```bash
sha256py "long text" --time
sha256py "debug" --log
```

---

#### Combined Example

```bash
sha256py -f input.txt --raw --time --log > output.txt
```
