# Changelog

All notable changes to this fork are documented in this file.

## [Unreleased]

### Added
- Forked from [wszqkzqk/PvZ-Portable](https://github.com/wszqkzqk/PvZ-Portable) at `848b1dd` into [interainjia/PvZ-Portable](https://github.com/interainjia/PvZ-Portable).
- `CHANGELOG.md` to track changes made in this fork.

### Notes
- Remotes: `origin` points to the fork, `upstream` to the original repository. Sync with `git pull upstream main`.
- Verified a local Windows build with MSYS2 UCRT64 (GCC, CMake, Ninja, SDL2, libpng, libjpeg-turbo, libopenmpt):
  ```
  cmake -G Ninja -B build -DCMAKE_BUILD_TYPE=Release
  cmake --build build
  ```
  Running requires `main.pak` and `properties/` from a legally purchased copy of PvZ GOTY next to the executable (or passed via `-resdir`), and `C:\msys64\ucrt64\bin` on `PATH` unless built with `-DBUILD_STATIC=ON`.
