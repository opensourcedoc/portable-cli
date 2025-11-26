# Portable CLI

A minimal layout for writing portable command-line tools.

This project separates platform-specific wrappers from the core logic:

- `bin/cli` — POSIX `sh` wrapper  
- `bin/cli.bat` — Windows batch wrapper  
- `libexec/cli.php` — core script (language-agnostic)

The wrapper handles:
- checking whether the required runtime exists  
- passing arguments through  
- returning the correct exit code  

The core script does not care about the operating system.

This repository shows one possible structure for writing small, portable CLI utilities without frameworks or dependencies.  
Replace `cli.php` with any language you prefer.

Nothing more.
