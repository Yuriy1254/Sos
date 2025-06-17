# 🧠 Sos — modified os-tutorial (x86‑64)

This project is my modification [cfenollosa/os-tutorial](https://github.com/cfenollosa/os-tutorial), adapted to the **x86‑64** architecture. I use the same structure: `00-environment`, `01-bootsector-barebones`, ..., gradually developing the system.

---

## 📦 Dependencies

### 🧱 Arch Linux

#### General packages

```bash
sudo pacman -S --needed base-devel git nasm qemu xorriso
```

#### i386-elf Toolchain

```bash
git clone https://aur.archlinux.org/i386-elf-gcc.git
cd i386-elf-gcc
makepkg -si

git clone https://aur.archlinux.org/i386-elf-binutils.git
cd i386-elf-binutils
makepkg -si
```

### 🧱 Debian / Ubuntu

#### General packages

```bash
sudo apt update
sudo apt install build-essential git nasm qemu-system-x86 xorriso
```

#### i386-elf Toolchain

```bash
sudo apt install gcc-i386
```


### 🧱 Fedora

#### General packages

```bash
sudo dnf install @development-tools git nasm qemu-system-x86 xorriso
```

#### i386-elf Toolchain

```bash
sudo dnf install gcc cross-binutils
```


---

## 📥 How to clone and work

```bash
git clone https://github.com/Yuriy1254/Sos.git
cd Sos
```
 - Open last version (23-fixes dir), than run

```bash
make clean
make run
```

---


## 🎯 The purpose of the project

- Boot from GRUB
- Protected Mode and C kernel
- Work with VGA text output
- Segmentation, interrupts, timers, keyboard
- In the future: support for ELF, syscall, multitasking



---

## 🙏 Thanks

- Original: [cfenollosa/os-tutorial](https://github.com/cfenollosa/os-tutorial)
- Documentation: [OSDev wiki](https://wiki.osdev.org/)

---

🧠 _If you want to learn system programming for real - go through these directories, collect code, change, break, and run again._

