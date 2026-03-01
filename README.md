# Milk-V Duo series buildroot SDK V2

```
./build.sh lunch
```

For more detailed documentation, please refer to: [https://milkv.io/docs/duo/getting-started/buildroot-sdk](https://milkv.io/docs/duo/getting-started/buildroot-sdk)

## Toolchain and C Library Versions

### Milk-V Duo 256M

The Duo 256M supports two build configurations:

| Configuration | Architecture | C Library | C Library Version | Toolchain |
|---|---|---|---|---|
| `milkv-duo256m-glibc-arm64-sd` | AArch64 (ARM64) | glibc | **2.25** | Linaro GCC 7.3.1-2018.05 (`aarch64-linux-gnu`) |
| `milkv-duo256m-musl-riscv64-sd` | RISCV64 | musl | — | GCC 10 (`riscv64-unknown-linux-musl`) |

The **glibc 2.25** version comes bundled with the Linaro GCC 7.3.1-2018.05 external toolchain (`gcc-linaro-7.3.1-2018.05-x86_64_aarch64-linux-gnu`).

