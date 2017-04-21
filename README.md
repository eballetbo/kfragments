# Kernel Configuration with Fragments

Kernel configuration can be done conveniently using configuration
fragments, which are small files that contain kernel configuration
options in the syntax of the original kernel's .config configuration
file.

## Linux Kernel Script

 scripts/Kconfig/merge_config.sh

## Linux Kernel Script Usage

To have the latest script usage information displayed please use the
command below in any linux kernel.

```
./scripts/Kconfig/merge_config.sh -h

```

Example:

```
./scripts/kconfig/merge_config.sh -m -r -O <LOGGING_DIRECTORY> <APPENDED_CONFIGs>
```

In this example:

```
-m  =  only merge the fragments, do not execute the make command
-n  =  use allnoconfig instead of alldefconfig
-r  =  list redundant entries when merging fragments
-O  =  dir to put generated output files
```

## Configuration files

Below is a list of configuration files that contain the configuration
flags that are not currently set in the specific defconfig.

* multi-v7 - Fragments to apply to multi_v7_defconfig
