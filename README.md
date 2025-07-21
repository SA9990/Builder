### 📥 Inputs
| - Name           | - Description                                                                |
|----------------|----------------------------------------------------------------------------|
| `user`         | GitHub username or organization that owns the kernel source repo           |
| `repo`         | Name of the repository containing the kernel source                        |
| `branch`       | Git branch to build from                                                   |
| `clang_type`   | Clang toolchain to use: `aosp` or `neutron`                                |
| `clang_url`    | URL to an AOSP Clang tar.gz (only required if using custom AOSP toolchain) |
| `config`       | Path to the kernel defconfig within the source repo                        |
| `LocalVersion` | Sets `CONFIG_LOCALVERSION` (e.g., `-custom`)                               |
| `cmd`          | Additional `make` flags (e.g. `"LD=ld.lld AR=llvm-ar NM=llvm-nm OBJCOPY=llvm-objcopy OBJDUMP=llvm-objdump READELF=llvm-readelf OBJSIZE=llvm-size STRIP=llvm-strip HOSTCC=clang HOSTCXX=clang++ -s"`)                                      |
| `ksu`          | Enable KernelSU if required                                                |

