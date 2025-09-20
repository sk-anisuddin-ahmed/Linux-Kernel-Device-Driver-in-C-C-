# 🧪 Linux Kernel Device Driver in C/C++

A personal exploration into Linux kernel module development using C/C++. This repository documents my journey from scratch—starting with basic character drivers and progressively diving into interrupt handling, memory-mapped I/O, and kernel-space debugging.

---

## 📌 Goals

- Understand kernel module lifecycle (`insmod`, `rmmod`, `modinfo`)
- Build a simple character device driver
- Log kernel messages using `printk`
- Compile modules with a reproducible `Makefile`
- Test modules in a minimal VM or WSL environment

---

## 🛠️ Getting Started

### Prerequisites

- Linux system (Ubuntu, Arch, or WSL2)
- Kernel headers installed (`linux-headers-$(uname -r)`)
- Basic C/C++ compiler (`gcc`, `make`)

### Build & Load

```bash
make           # Compile the kernel module
sudo insmod my_driver.ko   # Insert module
dmesg | tail   # Check kernel logs
sudo rmmod my_driver       # Remove module
