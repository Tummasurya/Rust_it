# How to Install Rust (Linux)

This guide walks through installing Rust and Cargo on a Linux system using `rustup`, the official toolchain installer.

## Prerequisites

- A Linux terminal with `curl` available
- `sudo` privileges (required only if a C compiler needs to be installed)

## 1. Install Rust via `rustup`

Run the official installation script:

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Follow the on-screen prompts to complete the installation. The default installation options are suitable for most users.

## 2. Configure the Environment

Once the installation finishes, load the Cargo environment variables into your current shell session:

```bash
source "$HOME/.cargo/env"
```

This step ensures the `rustc` and `cargo` commands are available without restarting the terminal.

## 3. Install a C Compiler (If Required)

Rust relies on a system linker to produce compiled binaries. Most Linux distributions already include one, but if you encounter linker errors during compilation, install the `build-essential` package:

```bash
sudo apt update && sudo apt install build-essential
```

## 4. Verify the Installation

Confirm that Rust and Cargo were installed correctly by checking their versions:

```bash
rustc --version
cargo --version
```

If both commands return version numbers, the installation was successful and you are ready to begin developing in Rust.
