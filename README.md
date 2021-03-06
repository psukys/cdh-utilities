# cdh-utilities
This repository contains utilities that support different tasks around MOVE-II's CDH platform.

---

## SPI Parallel Access Test
Tests for the SPI interface. For more information read the README.md in the spi-parallel-access-test directory.

---

## moveio

Contains a C++ Wrapper Library for IO functions (SPI, GPIO, PinMapper). For more information read the README.md in the moveio directory.

---

## create\_image.sh
This tool creates a complete Linux image from the yocto build artifacts (i.e. rootfs, kernel, kernel-modules, ...).

### Usage
```bash
./create_image.sh [options] deploy_dir
```

* *deploy\_dir*

    The path to the yocto image deploy directory, in which the build artifacts are located.

### Options
* *-i image_name*

    Name of the image that you want to create the image file for. Defaults to _core-image-cdh_.

* *-s rootfs_size*

    Size of the rootfs partition in megabytes. Defaults to _128_.
