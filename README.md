Brand new pintos for Operating Systems and Lab (CS330), KAIST, by Youngjin Kwon.

The manual is available at https://casys-kaist.github.io/pintos-kaist/.

----

## Apple Silicon Support

This repository supports Apple Silicon (M1) Macs. If you are using an Apple Silicon Mac, please follow the instructions below. It's inspired by [pintos_mac repository](https://github.com/maojie/pintos_mac)

### 1. Install Homebrew
    
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### 2. Install QEMU

```bash
brew install qemu
```

### 3. Install GCC Cross Compiler

```bash
brew install binutils make        # This is required for x86_64-elf-gcc@7
brew install x86_64-elf-binutils  # This is required for x86_64-elf-gcc@7

curl -O https://gist.githubusercontent.com/hey-jude/e272aa2f35f89ecf599572a0d11db618/raw/cff9718ec9da0f8fe109b284e0ccfbab0f87d95a/x86_64-elf-gcc@7.rb
brew install --build-from-source x86_64-elf-gcc@7.rb
```

### 4. Install GDB (Optional)

```bash
brew install x86_64-elf-gdb
```