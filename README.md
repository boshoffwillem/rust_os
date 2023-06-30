# rust_os

To build the program run

```bash
cargo bootimage
```

To run the program on Windows

```bash
qemu-system-x86_64 -drive format=raw,file=target/x86_64-rust_os/debug/bootimage-rust_os.bin
```
