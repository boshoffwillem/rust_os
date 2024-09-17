# rust_os

Prerequisites:

```bash
rustup toolchain install nightly-x86_64-pc-windows-gnu
rustup default nightly-x86_64-pc-windows-gnu
```

```bash
rustup component add rust-src --toolchain nightly-x86_64-pc-windows-gnu
```

```bash
rustup target add x86_64-unknown-none
```

```bash
rustup component add llvm-tools-preview
```

```bash
cargo install bootimage
```

To build the program run

```bash
cargo bootimage
```

To run the program on Windows

```bash
qemu-system-x86_64 -drive format=raw,file=target/x86_64-rust_os/debug/bootimage-rust_os.bin
```
