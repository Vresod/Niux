## Niux: Another Kernel
Kernel built in Pure Assembly, and C


## What does it do?

It does kernel things


# Development

## How do you build?

```
cd src
./build.sh
````

You're gonna need these dependencies for building:

- Grub
- Mtools
- Xorriso
- Nasm
- Binutils

You're also gonna want to build the i686-elf toolchain with

```
./toolchain.sh
```

## What are the dependencies I need?

- Grub
- Mtools
- Xorriso
- Nasm
- Binutils
- qemu
- (if you run arch, this is required. Not sure about other distros.) qemu-arch-extra

## Running the kernel

### On real hardware
```
sudo dd if=niux.iso of=[device] bs=4M
```

### With QEMU
```
qemu-system-i386 -cdrom niux.iso
```
