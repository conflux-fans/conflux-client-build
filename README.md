# conflux-client-build

Daily automatic build of Conflux-rust client.

> Warning: that the build is based on the master branch and is intended for developers only. If you need to run the official client, please download it from the [release](https://github.com/Conflux-Chain/conflux-rust/releases).

# Usage

This project automatically checks for new commits in conflux-rust daily. If any are found, an automatic build will be triggered, and you can download the latest conflux build from the [release](https://github.com/conflux-fans/conflux-client-build/releases).

# Troubleshooting

## Windows

- The program can't start because MSVCP140D.DLL is missing from your computer. Try reinstalling the program to fix this problem
- The code execution cannot proceed because VCRUNTIME140_1.dll was not found. Reinstalling the program may fix this problem.

- The code execution cannot proceed because VCRUNTIME140.dll was not found. Reinstalling the program may fix this problem.

You need the [Microsoft Visual C++ Redistributable Version](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170)


- The code execution cannot proceed because LIBCRYPTO-3-x64.dll was not found. Reinstalling the program may fix this problem.
- The code execution cannot proceed because LIBSSL-3-x64.dll was not found. Reinstalling the program may fix this problem.

```ps
choco install openssl -y
```

## Linux

- error while loading shared libraries: libssl.so.3

```bash
apt install openssl -y
```

- error while loading shared libraries: libsqlite3.so.0

```bash
apt install sqlite3 -y
```

# Supported by @xcfx-node

This project is supported by [@xcfx-node](https://github.com/iosh/xcfx-node), which is a Node.js binding for [Conflux-rust](https://github.com/Conflux-Chain/conflux-rust)
