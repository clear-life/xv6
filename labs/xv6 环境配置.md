# xv6 环境配置

**环境**

wsl ubuntu24.04

**更新软件**

```bash
sudo apt-get update && sudo apt-get upgrade
```

**安装 xv6 环境**

*   git 版本控制工具
*   build-essential 开发工具集合
*   gdb-multiarch 支持多 CPU 架构的 gdb
*   qemu-system-misc qemu 系统模拟器集合
*   gcc-riscv64-linux-gnu RISC-V 64位交叉编译器, 能在x86-64位机器上编译出 RISC-V 程序
*   binutils-riscv64-linux-gnu RISC-V 版的二进制工具集

```bash
sudo apt-get install git build-essential gdb-multiarch qemu-system-misc gcc-riscv64-linux-gnu binutils-riscv64-linux-gnu
```

**测试**

```bash
qemu-system-riscv64 --version
```

至少一个基于 RISC-V 的 GCC

```bash
riscv64-linux-gnu-gcc --version
riscv64-unknown-elf-gcc --version
riscv64-unknown-linux-gnu-gcc --version
```





