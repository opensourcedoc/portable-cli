# Portable CLI

A minimal layout for writing portable command-line tools.

This project separates platform-specific wrappers from the core logic:

* *bin/cli*         — POSIX sh wrapper
* *bin/cli.bat*     — Windows batch wrapper
* *libexec/cli.php* — core script (language-agnostic)

The wrapper is responsible for:

* Checking whether the required runtime exists
* Passing command-line arguments through
* Returning the correct exit code

The core script does not care about the operating system.

This repository demonstrates one possible structure for writing small, portable CLI utilities without frameworks or dependencies.

Replace `cli.php` with any language you prefer.

Nothing more.
