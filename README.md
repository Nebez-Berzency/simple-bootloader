# Simple Bootloader

A minimal x86 bootloader written in Assembly.

This project is part of my low-level programming journey and is designed to help me understand how the PC boot process works, from BIOS to Real Mode execution.

---

## ✨ Features

- Written in x86 Assembly (NASM)
- Boots in 16-bit Real Mode
- Uses BIOS interrupt `0x10` for screen output
- Prints a simple message to the screen
- Compatible with QEMU
- Educational project

---

## 🎯 Learning Goals

This project is built to explore and understand:

- The PC boot process
- BIOS services
- x86 Real Mode programming
- Memory layout during boot
- Bootloader fundamentals

---


## 📖 Article
- 🇬🇧 English: [Building a Bootloader from Scratch](https://dev.to/nebez/building-a-bootloader-from-scratch-53ea)
- 🇮🇷 Persian: [اولین تجربه من در دنیای Low-Level Programming؛ ساخت اولین Bootloader](https://vrgl.ir/XPQrg)
---

### 📁 Project Structure

```text
simple-bootloader/
├── src/
│   └── boot.asm
└── README.md
```

---

## 🚀 Getting Started

Follow these steps to build and run the project on your local machine.

### 📦 Prerequisites

Install the required tools:

#### Ubuntu / Debian

```bash
sudo apt update
sudo apt install nasm qemu-system-x86
```

---

## 📥 Clone the Repository

```bash
git clone https://github.com/Nebez-Berzency/simple-bootloader.git
cd simple-bootloader
```

---

## 🔨 Build

Compile the bootloader using NASM:

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

- [x] Boot from BIOS
- [x] Print text using BIOS interrupt `0x10`
- [ ] Print colored text
- [ ] Handle keyboard input
- [ ] Explore additional BIOS interrupts

---

## 📜 License

Copyright (c) 2026 Nebez Berzency

Licensed under the **MIT License**.

Feel free to use, modify, and learn from this project.

---

> Keep coding. Keep building. 🚀
