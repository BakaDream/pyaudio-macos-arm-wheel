# PyAudio Mac ARM Wheel

[Englisth](https://github.com/BakaDream/pyaudio-macos-arm-wheel/blob/main/README.md) [简体中文](https://github.com/BakaDream/pyaudio-macos-arm-wheel/blob/main/README_zh-cn.md)
## 项目介绍

这是为 **macOS ARM（Apple Silicon）** 提供的 **PyAudio 预编译 wheel 包**。  
已内置 PortAudio，无需自行编译，即可直接安装。

仓库地址：[https://github.com/BakaDream/pyaudio-macos-arm-wheel](https://github.com/BakaDream/pyaudio-macos-arm-wheel)


## 目录

- [快速开始](#快速开始)
- [下载与安装](#下载与安装)
  - [使用 pip 安装](#使用-pip-安装)
  - [使用 uv 安装](#使用-uv-安装)
- [测试安装](#测试安装)

## 快速开始

1. 访问 [Releases 页面](https://github.com/BakaDream/pyaudio-macos-arm-wheel/releases/latest)。
2. 找到对应 Python 版本的 PyAudio wheel，例如 Python 3.12 对应 cp312。
3. 复制下载链接，使用 pip 或 uv 安装。
4. 测试安装，确认 PyAudio 正常工作。

## 下载与安装

### 使用 pip 安装

```bash
pip install <对应 wheel 链接>
````

示例 (Python 3.12):

```bash
pip install https://github.com/BakaDream/pyaudio-macos-arm-wheel/releases/download/v1.0.1/pyaudio-0.2.14-cp312-cp312-macosx_11_0_arm64.whl
```

### 使用 uv 安装

> **提示**: `uv` 是支持自定义 PyPI 源的 Python 包管理工具。

```bash
uv pip install <对应 wheel 链接>
```

示例 (Python 3.12):

```bash
uv pip install https://github.com/BakaDream/pyaudio-macos-arm-wheel/releases/download/v1.0.1/pyaudio-0.2.14-cp312-cp312-macosx_11_0_arm64.whl
```

## 测试安装

```python
import pyaudio

p = pyaudio.PyAudio()
print("PyAudio 初始化成功！", p)
p.terminate()
```

输出示例:

```
PyAudio 初始化成功！ <pyaudio.PyAudio object at 0x...>
```

🌟如果这个项目对你有帮助，欢迎在 GitHub 仓库点个 Star🌟 支持一下，非常感谢！
