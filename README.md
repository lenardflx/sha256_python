<div align="center">
<pre>
███████ ██   ██  █████  ██████  ███████  ██████  ██████  ██    ██ 
██      ██   ██ ██   ██      ██ ██      ██       ██   ██  ██  ██  
███████ ███████ ███████  █████  ███████ ███████  ██████    ████   
     ██ ██   ██ ██   ██ ██           ██ ██    ██ ██         ██    
███████ ██   ██ ██   ██ ███████ ███████  ██████  ██         ██    
-----------------------------------------------------------------
A pure Python implementation of the SHA-256 hashing algorithm.
</pre>

[![PyPI version](https://badge.fury.io/py/sha256py.svg)](https://pypi.org/project/sha256py/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

</div>

---

## Installation

### From PyPI (recommended)

```bash
pip install sha256py
```

### From source

```bash
git clone https://github.com/lenardflx/sha256_python.git
cd sha256_python
pip install -e .
```

---

## Usage

### As library

```python
from sha256py import Sha256

my_hash = Sha256("Hello World!")
print(my_hash.hexdigest())
```

### As command line tool

```bash
# Prompted input
sha256py

# Hash from cli input
sha256py "hello world"

# Save output to file
sha256py "data" > hash.txt
```

---

## Testing

This project uses `pytest` for testing.

```bash
# Install pytest
pip install pytest

# Run all tests
pytest
```

---

## Contributing

Feel free to contribute! Here is how to do it:

1. Fork the repository (https://github.com/lenardflx/sha256_python/fork)
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Make your changes 
4. Commit your changes (`git commit -m 'Add some feature'`)
5. Push to the branch (`git push origin feature/your-feature`)
6. Create a new Pull Request

---

## License & Metadata

Lenard Felix - [contact@lenardfelix.de](mailto:contact@lenardfelix.de)  

This project is licensed under MIT. See [LICENSE](LICENSE) for details.

Compatible with Python 3.7 and above.