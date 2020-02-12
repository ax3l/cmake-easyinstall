# cmake-easyinstall ![Supported Platforms](https://img.shields.io/badge/platforms-linux%20|%20osx-blue.svg)

Install CMake projects as simple as you love it from pip:
```sh
cmake-easyinstall git+https://github.com/org/rego.git
```

![cmake-easyinstall demo](cmake_easyinstall_opt.gif)

## Install

```sh
curl -L -o cmake-easyinstall https://git.io/JvLxY
chmod a+x cmake-easyinstall
```

## Usage

```sh
cmake-easyinstall git+<https-url>.git [cmake-options]
```

## Dependencies

- bash
- cmake 3.12.0+
- curl (for the initial download)
- git
- ninja, make, or any other [native build system](https://cmake.org/cmake/help/v3.16/manual/cmake-generators.7.html)
