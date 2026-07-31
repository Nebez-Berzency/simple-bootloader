# Simple Bootloader

A minimal x86 bootloader written in Assembly.

This project is part of my low-level programming journey and is designed to help understand how the PC boot process works. It focuses on learning the fundamentals of BIOS, Real Mode, and bootloader development.

---

## ✨ Features

* Written in x86 Assembly (NASM)
* BIOS bootable
* Runs in Real Mode (16-bit)
* Compatible with QEMU
* Educational and beginner-friendly

---

## 📁 Project Structure

```text
simple-bootloader/
├── src/
│   └── boot.asm
├── bin/
├── Makefile
└── README.md
```

---

## 🚀 Getting Started

Follow these steps to build and run the project on your local machine.

### 📦 Prerequisites

Install the required build tools and emulator.

#### Ubuntu / Debian

```bash
sudo apt update
sudo apt install nasm qemu-system-x86 make
```

---

## 📥 Clone the Repository

```bash
git clone https://github.com/Nebez-Berzency/simple-bootloader.git
cd simple-bootloader
```

---

## 🔨 Build

If you are using the Makefile:

```bash
make
```

Or compile manually with NASM:

```bash
nasm -f bin src/boot.asm -o bin/boot.bin
```

---

## ▶️ Run

Boot the generated binary with QEMU:

```bash
qemu-system-x86_64 -drive format=raw,file=bin/boot.bin
```

---

## 🗺️ Roadmap

* Print colored text
* Keyboard input
* Memory detection
* Simple command prompt
* Basic file loading

---

## 📜 License

Copyright (c) 2026 Nebez Berzency

This project is licensed under the **MIT License**.

Feel free to use, modify, and distribute it for educational purposes.

---

> Keep coding. Keep building. 🚀
