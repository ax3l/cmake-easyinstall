# cmake-easyinstall ![Supported Platforms](https://img.shields.io/badge/platforms-linux%20|%20osx%20|%20windows-blue.svg) ![License: BSD-2-Clause](https://img.shields.io/github/license/ax3l/cmake-easyinstall)

Install CMake projects as simple as:
```sh
cmake-easyinstall git+https://github.com/org/repo.git
```

![cmake-easyinstall demo](cmake_easyinstall_opt.gif)

## Install

```sh
curl -L -o cmake-easyinstall https://git.io/JvLxY
chmod a+x cmake-easyinstall
```

## Usage

```sh
cmake-easyinstall [--prefix=<dir>] git+<https-url>.git [cmake-options]
```

## Environment Options

Just `export CEI_<option>=<value>` to change some defaults:

- `CEI_CMAKE`: path or alias for the cmake command (default: `cmake`)
- `CEI_CONFIG`: the [build configuration](https://cmake.org/cmake/help/v3.16/manual/cmake.1.html#build-tool-mode) (default: `RelWithDebInfo`)
- `CEI_PARALLEL`: maximum number of concurrent build processes (default: `2`)
- `CEI_PREFIX`: installation prefix (default: CMake default)
- `CEI_SUDO`: set to `"sudo"` for privileged installation (default: "")

# Command Line Options

- `--prefix=<dir>`: installation prefix (default: CMake default)

Note: `cmake-options` take precedence over `--prefix` takes precedence over environment options.

## Dependencies

- bash
- cmake 3.12.0+
- git
- ninja, make, or any other [native build system](https://cmake.org/cmake/help/v3.16/manual/cmake-generators.7.html)
