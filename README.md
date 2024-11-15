# Fortran and Meson Template for VSCode

This repository is a template for setting up a modular Fortran project using Visual Studio Code (VSCode), Meson build system, and Ninja. It includes basic project files to help developers get started with Fortran, Meson, and debugging in VSCode. 

## Prerequisites
Ensure the following tools are installed:

- **Fortran Compiler**: Verify installation by checking the compiler version (e.g., `gfortran --version`).
- **Meson**: Used as the build system. Check installation with:
```bash
meson --version
```
- **Ninja**: A high-speed build tool. Verify installation with:
```bash
ninja --version
```

## Quickstart 

### Get modern Fortran Extension for VSCode

This provides syntax highlighting, code navigation, and debugging support for Fortran. Install via pressing `Ctrl+Shift+P` and:
```bash
ext install fortran-lang.linter-gfortran
```


### Clone this repository

```bash
git clone https://github.com/tornikeo/fortran-meson-ninja-vscode-template.git
cd fortran-meson-ninja-vscode-template
```
### Build and Debug
1. Open [main.f90](./src/main/main.f90) in VSCode.
2. Set a breakpoint by clicking next to the line number where you want execution to pause.
3. Press `F5` to start debugging.

Alternatively, you can run the executable manually from the command line:
```bash
./build/main.exe
```

## Customizing for Additional Modules

If you add extra directories or modules, update `.vscode/settings.json` to ensure VSCode’s IntelliSense picks up the new paths. After updating, restart the Fortran language server by opening the Command Palette (`Ctrl+Shift+P`), typing "Fortran: Restart Language Server," and pressing Enter.

## License
This project is licensed under the MIT License. See the [LICENSE.txt](LICENSE.txt) file for more details.
