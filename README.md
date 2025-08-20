# PyAudio Mac ARM Wheel

[Englisth](https://github.com/BakaDream/pyaudio-macos-arm-wheel/blob/main/README.md) [简体中文](https://github.com/BakaDream/pyaudio-macos-arm-wheel/blob/main/README_zh-cn.md)
## Project Introduction

This is a **precompiled PyAudio wheel package** for **macOS ARM (Apple Silicon)**.  
It comes with PortAudio built-in, so you can install it directly without compiling PortAudio yourself.

Repository URL: [https://github.com/BakaDream/pyaudio-macos-arm-wheel](https://github.com/BakaDream/pyaudio-macos-arm-wheel)


## Table of Contents

- [Quick Start](#quick-start)
- [Download and Installation](#download-and-installation)
  - [Install with pip](#install-with-pip)
  - [Install with uv](#install-with-uv)
- [Test the Installation](#test-the-installation)

## Quick Start

1. Visit the [Releases page](https://github.com/BakaDream/pyaudio-macos-arm-wheel/releases/latest).
2. Find the PyAudio wheel corresponding to your Python version, e.g., cp312 for Python 3.12.
3. Copy the download link and install using pip or uv.
4. Test the installation to confirm that PyAudio works properly.

## Download and Installation

### Install with pip

```bash
pip install <corresponding wheel link>
````

Example (Python 3.12):

```bash
pip install https://github.com/BakaDream/pyaudio-macos-arm-wheel/releases/download/v1.0.1/pyaudio-0.2.14-cp312-cp312-macosx_11_0_arm64.whl
```

### Install with uv

> **Note**: `uv` is a Python package management tool that supports custom PyPI sources.

```bash
uv pip install <corresponding wheel link>
```

Example (Python 3.12):

```bash
uv pip install https://github.com/BakaDream/pyaudio-macos-arm-wheel/releases/download/v1.0.1/pyaudio-0.2.14-cp312-cp312-macosx_11_0_arm64.whl
```

## Test the Installation

```python
import pyaudio

p = pyaudio.PyAudio()
print("PyAudio initialized successfully!", p)
p.terminate()
```

Example output:

```
PyAudio initialized successfully! <pyaudio.PyAudio object at 0x...>
```



🌟If this project has been helpful to you, please consider giving it a Star🌟 on the GitHub repository. Your support is greatly appreciated!