## Build & Run -
- bash
- make                          # Compile the module
- sudo insmod hello_sk.ko       # Insert the module
- dmesg | tail                  # View kernel logs
- sudo rmmod hello_sk           # Remove the module

## Useful Commands -
- bash
- lsmod                         # List loaded modules
- modinfo hello_sk.ko           # Show module info
- cat /proc/devices             # View registered devices