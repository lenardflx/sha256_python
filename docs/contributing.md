## Contributing Guide

The project won't be actively maintained by me, but I welcome contributions.
This is also great to learn how SHA256 works!

---

### How to Contribute

> This assumes basic familiarity with Git and GitHub. If you're new, I recommend GitHub's [Hello World Guide](https://docs.github.com/en/get-started/quickstart/hello-world).

#### 1. Fork the repository

Go to the GitHub repo and click the ["Fork"](https://github.com/lenardflx/sha256_python/fork) button in the top right corner.
This creates your own copy in your account.


#### 2. Clone your fork to your computer

```bash
git clone https://github.com/<your_username>/sha256_python
cd sha256_python
```

Or use the GUI of your IDE (e.g. PyCharm).


#### 3. Set up a branch for your changes

```bash
git checkout -b feature/your-feature
```

I recommend using a descriptive name for your branch, like `feature/better-log-output`.


#### 4. Make your changes

* Open the project in your IDE
* Modify the code as needed


#### 5. Test your changes

This project uses `pytest` for testing. Make sure you have it installed:

```bash
pytest --version
```
If not, install it:

```bash
pip install pytest
```

Tests are located in the `tests/` directory:

* `test_core.py`
* `test_utils.py`
* `test_cli_behavior.py`

Add new tests accordingly.

To run the tests:

```bash
pytest
```


#### 6. Commit your changes

```bash
git add .
git commit -m "Add: better log output for --log flag"
```


#### 7. Push changes to your fork

```bash
git push origin feature/your-feature
```


#### 8. Create a Pull Request

* Go to your fork on GitHub
* Click **"Compare & pull request"**
* Add a title and description

Tests are located in the `tests/` directory, split into logical modules:

* `test_core.py`
* `test_utils.py`
* `test_cli_behavior.py`

Add new tests where relevant.

---

Thanks for considering contributing to this project! 💜
