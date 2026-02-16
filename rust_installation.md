# **Rust Installation Documentation**
This is guide to install **Rust Programming Language** for Windows with *GNU toolchain*, instead of default proprietary *Microsoft Visual Studio 2019 for build tools*.

---

## Downloads
- Rust Installer: https://rust-lang.org/tools/install/
- MSYS2 Installer: https://www.msys2.org/

---

## Rust Installation

### 1. Download Official Rust Installer for Windows
https://rust-lang.org/tools/install/

---

### 2. Run the installed executable file

#### New terminal session will be launched and follow the steps:
``` text
1) Proceed with standard installation (default - just press enter)
2) Customize installation
3) Cancel installation
```
> Choose option *"2"*, this enables GNU Toolchain.

```bash
I'm going to ask you the value of each of these installation options. You may simply press the Enter key to leave unchanged.
Default host triple? [x86_64-pc-windows-msvc]
```
> Enter *"x86_64-pc-windows-gnu"*, for GNU toolchain.

```bash
Default toolchain? (stable/beta/nightly/none) [stable]
```
> For the stable release, Enter *"stable"* or just press Enter.

```bash
Profile (which tools and data to install)? (minimal/default/complete) [default]
```
> Enter *"default"* or just press Enter for the default tools (i.e; compiler, package manager etc.)

```bash
Modify PATH variable? (Y/n)
```
> Enter *"y"*, for global installation.

```bash
Current installation options: 
default host triple: x86_64-pc-windows-gnu default 
toolchain: stable 
profile: default 
modify PATH variable: yes 

1) Proceed with selected options (default - just press enter) 
2) Customize installation 
3) Cancel installation
```
> Proceed with the customized installation, Enter *"1"*

```bash
info: default toolchain set to 'stable-x86_64-pc-windows-gnu' 
stable-x86_64-pc-windows-gnu installed - (timeout reading rustc version) 

Rust is installed now. Great! 

To get started you may need to restart your current shell. This would reload its PATH environment variable to include Cargo's bin directory (%USERPROFILE%\.cargo\bin). 

Press the Enter key to continue.
```
> Press Enter.
Terminal will close and that is expected.

### 4. Launch a new terminal session.

```bash
rustc --version
cargo --version
rustup show
```
To test if the rust is installation was successful or not.

---

## Tools Installation using MSYS2

### 5. Install MSYS2 for GNU tools (GCC)
[MSYS2](https://www.msys2.org/)

### 6. Close all terminal sessions and Launch "MSYS2 MinGW 64"
```bash
pacman -Syu
```
> To update tool packages

```bash
pacman -S mingw-w64-x86_64-gcc
```
> To install GCC

---

## System Environment Variables

### 7. Open *"Edit the system environment variables"*
- Click "Environment Variables..." at the bottom right.
- Under "User Variables for <Username>", locate "Path".
- Select, Edit and Add "folder path for GCC binaries".
- GCC folder path default 
    ```text
    "C:\msys64\mingw64\bin"
    ```
- Add then OK all windows

New Terminal session to check installation of GCC and G++ tools.
```bash
gcc --version
g++ --version
```

## Now Rust is all set.
