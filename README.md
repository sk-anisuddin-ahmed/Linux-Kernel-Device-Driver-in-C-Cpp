# 🧪 Linux Kernel Device Driver in C/C++

A personal exploration into Linux kernel module development - device driver development. 
This repository documents my journey from scratch—starting with basic character drivers and 
progressively diving into interrupt handling, memory-mapped I/O, and kernel-space debugging.

---

## 📌 Goals

- Understand kernel module lifecycle (`insmod`, `rmmod`, `modinfo`, `modprobe`)
- Build a simple character device driver
- Log kernel messages using `printk` `pr_info`
- Compile modules with a reproducible `Makefile`
- Test modules in a minimal Virtual environment - (Multipass, WSL)

---

## 🛠️ Getting Started

### Prerequisites

- Linux system (Ubuntu, Arch or WSL2)
- Kernel headers installed (`linux-headers-$(uname -r)`)
- Basic C compiler (`gcc`, `make`)

### Build & Load

```bash
make           				# Compile the kernel module
sudo insmod my_driver.ko   	# Insert module
dmesg | tail   				# Check kernel logs
sudo rmmod my_driver       	# Remove module
```