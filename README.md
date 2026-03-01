# Milk-V Duo series buildroot SDK V2

```
./build.sh lunch
```

For more detailed documentation, please refer to: [https://milkv.io/docs/duo/getting-started/buildroot-sdk](https://milkv.io/docs/duo/getting-started/buildroot-sdk)

## Toolchain and C Library Versions

### Milk-V Duo 256M

The Duo 256M supports two build configurations:

| Configuration | Architecture | C Library | GCC Version | Toolchain |
|---|---|---|---|---|
| `milkv-duo256m-glibc-arm64-sd` | AArch64 (ARM64) | glibc 2.25 | **7.3.1** | Linaro GCC 7.3.1-2018.05 (`aarch64-linux-gnu`) |
| `milkv-duo256m-glibc-arm64-sd-gcc14` | AArch64 (ARM64) | glibc 2.39+ | **14.2** | ARM official GCC 14.2.rel1 (`aarch64-none-linux-gnu`) |
| `milkv-duo256m-musl-riscv64-sd` | RISCV64 | musl | 10.x | GCC 10 (`riscv64-unknown-linux-musl`) |

The `milkv-duo256m-glibc-arm64-sd-gcc14` configuration uses the [ARM official GNU Toolchain 14.2.rel1](https://developer.arm.com/open-source/gnu-toolchain), which is downloaded automatically by buildroot. It provides GCC 14 with a more recent glibc, offering support for newer C/C++ standards and improved optimisations compared to the Linaro 7.3.1 configuration.

