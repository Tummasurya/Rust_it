# Rust Hello World

This guide covers creating, compiling, and running your first Rust program.

## Prerequisites

Before proceeding, ensure Rust is installed on your system. See [How to Install Rust (Linux)](How_to_Install_Rust__Linux_.md) for setup instructions.

## 1. Create the Project

Use Cargo, Rust's build tool and package manager, to scaffold a new project:

```bash
cargo new hello_world
```

This command generates a project directory containing a `Cargo.toml` manifest file and a `src` subdirectory:

```
~/rust/hello_world$ ls
Cargo.toml  src/
```

## 2. Compile `main.rs`

Navigate to the `src` directory and compile the source file directly using `rustc`:

```bash
cd src/
rustc main.rs
```

This produces an executable alongside the source file:

```
~/rust/hello_world/src$ ls
main*  main.rs
```

> **Note:** `rustc` compiles a single file and does not manage project dependencies. For multi-file or dependency-based projects, use `cargo build` instead.

## 3. Run the Executable

Execute the compiled binary:

```bash
./main
```

**Expected output:**

```
Hello, world!
```

With that, your first Rust program is up and running.
