# Basic Calculator with GUI in C

This project is a simple calculator with a graphical user interface (GUI) built using the GTK library. The calculator supports basic arithmetic operations such as addition, subtraction, multiplication, division, modulus, exponentiation, and square root.

## Features

- **GUI-Based:** Easy-to-use graphical user interface.
- **Advanced Operations:** Supports basic arithmetic, modulus, exponentiation, and square root.
- **Windows-Compatible:** This guide is tailored for Windows users.

## how to download the repo first time users

- click link to read [**Instructions**](https://www.gitprojects.fnbubbles420.org/how-to-download-repos)

## Prerequisites

To compile and run this program on Windows, you need to set up the GTK environment using MSYS2.

### Step 1: Install MSYS2

1. Download and install MSYS2 from the official website: [MSYS2](https://www.msys2.org/).
2. After installation, open the MSYS2 terminal.

### Step 2: Install GTK and GCC

Update the package database and install the necessary packages:

```
pacman -Syu
pacman -S mingw-w64-x86_64-gtk3 mingw-w64-x86_64-gcc
```

### Step 3: Download the Source Code
- Download the `calculator.c` file directly from the provided source.
- Save the file to a directory of your choice on your local machine.

### Step 4: Compile the Program
- Open the MSYS2 MinGW 64-bit terminal and navigate to the directory where you saved `calculator.c`. Compile the program using the following command:

```
gcc calculator.c -o calculator.exe `pkg-config --cflags --libs gtk+-3.0`
```

### Step 5: Run the Program
- Once compiled, you can run the program directly from the terminal or by double-clicking `calculator.exe` in your file explorer.

```
./calculator.exe
```


## Notes

- **GTK Libraries:** Ensure that the required GTK DLLs are accessible in your system's PATH, or place them in the same directory as your compiled `.exe` file. These DLLs are part of the GTK installation handled by MSYS2.
- **Packaging:** If you plan to distribute the executable, include the necessary GTK runtime DLLs with it.

## Troubleshooting

- **Missing DLLs:** If the program doesn't start due to missing DLLs, ensure all GTK runtime libraries are included or properly referenced in your PATH.
- **Compilation Errors:** Make sure you are using the MinGW 64-bit terminal in MSYS2 and have installed the correct packages.



