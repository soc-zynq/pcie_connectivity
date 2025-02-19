# pcie_connectivity

## Description
A simple kernel module with a user-space application.

## Project Structure
```
pcie_connectivity/
├── kernel_module/
│   ├── src/
│   │   └── pcie_connectivity.c
│   ├── include/
│   │   └── pcie_connectivity.h
│   └── Makefile
└── application/
    ├── main.c
    └── CMakeLists.txt
```

## Build

### Kernel Module
```bash
cd pcie_connectivity/kernel_module
make
```

### Application
```bash
cd pcie_connectivity/application
cmake .
make
```

## Usage

### Kernel Module
```bash
sudo insmod pcie_connectivity/kernel_module/pcie_connectivity.ko
# Do something with the module
sudo rmmod pcie_connectivity
```

### Application
```bash
cd pcie_connectivity/application
./test_app
```

## License
GPL
