# riscv-tools-bin
> for self-use backup.

self-use riscv-gnu-toolchain, riscv-isa-sim and pk bin files collection.

## Include
1. [riscv-gnu-toolchain](https://github.com/riscv-collab/riscv-gnu-toolchain)
2. [riscv-isa-sim](https://github.com/riscv-software-src/riscv-isa-sim)
3. [riscv-pk](https://github.com/riscv-software-src/riscv-pk)

## Platform
Debian GNU/Linux 11

## Arch
aarch64

## uname -a
Linux 3ed4a8f831cf 5.15.49-linuxkit #1 SMP PREEMPT Tue Sep 13 07:51:32 UTC 2022 aarch64 GNU/Linux

## Usage
1. uncompress.
> eg. uncompress to /wks/riscv-tools

2. add to `PATH` variable.
> eg. add to `~/.bashrc`
```bash
export PATH=$PATH:/wks/riscv-tools/bin
```

3. apply `PATH` variable.
```bash
source ~/.bashrc
```

4. add `hello.c` and test.

```bash
riscv64-unknown-elf-gcc -o hello hello.c

spike pk hello
```

5. enjoy.
