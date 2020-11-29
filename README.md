# version_util

Simple version utility shell.

## Goal

It is tiresome to updating libraries in Dockerfile.
To automate it, we need a script to check latest version of those libraries.

This script's goal is to process version for automation.

## How to use

Copy or source version_util.sh and run function.

```bash
source version_util.sh

java_ver=$(get_library_ver_dockerfile JAVA)
inc_java_ver=$(increment_simple_version ${java_ver})
# use ${inc_java_ver} for checking whether new version exists
```
