# Python Virtual Environment (venv) Guide

![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![Platform](https://img.shields.io/badge/platform-All%20Platforms-lightgrey)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

This repository contains a simple guide on how to create and use Python virtual environments using `venv`. A virtual environment helps you manage project-specific dependencies without affecting your global Python installation.

---

## Table of Contents

- [Requirements](#requirements)
- [Creating a Virtual Environment](#creating-a-virtual-environment)
- [Activating the Virtual Environment](#activating-the-virtual-environment)
- [Installing Packages](#installing-packages)
- [Deactivating the Virtual Environment](#deactivating-the-virtual-environment)
- [Deleting a Virtual Environment](#deleting-a-virtual-environment)

---

## Requirements

- Python 3.3 or higher
- `venv` module (comes built-in with Python 3.3+)

Check your Python version:

```bash
python3 --version
```

## Creating a Virtual Environment

Navigate to your project folder and run:

```bash
python3 -m venv venv
```

This will create a folder named `venv` in your project directory containing the virtual environment.

## Activating the Virtual Environment

### On macOS/Linux:

```bash
source venv/bin/activate
```

### On Windows (Command Prompt):

```bash
venv\Scripts\activate
```

### On Windows (PowerShell):

```bash
venv\Scripts\Activate.ps1
```

Once activated, your terminal prompt will show `(venv)` before the path.

## Installing Packages

With the virtual environment active, you can install packages using `pip`:

```bash
pip install <package_name>
```

You can also save your dependencies to a `requirements.txt` file:

```bash
pip freeze > requirements.txt
```

And install from it later:

```bash
pip install -r requirements.txt
```

## Deactivating the Virtual Environment

To deactivate, simply run:

```bash
deactivate
```

## Deleting a Virtual Environment

If you want to remove the virtual environment, just delete the `venv` folder:

```bash
rm -rf venv  # macOS/Linux
rmdir /s /q venv  # Windows
```

## License

No License considering this is general knowledge.
