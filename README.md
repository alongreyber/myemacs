# Overview

This is my emacs editor configuration. It's very opinionated and set up for personal use.

# Setup

I've tried to make the configuration as declarative as possible so that it's easy to install reliably.

## Install Emacs

I recently switched to GccEmacs, which compiles all Elisp to C ahead of time. There is an initial time required for compilation but I've noticed a performance improvement afterwards.

### Mac OS

This is easy on MacOS thanks to the emacs-plus package:

```
brew tap d12frosted/emacs-plus
brew install emacs-plus@28 --with-native-comp
```

### Ubuntu

TODO

## Install Spacemacs

```
git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d
```

## Symlink spacemacs configuration from this repo

This keeps your .spacemacs file in version control.

```
ln ~/myemacs/spacemacs.el ~/.spacemacs
```

## Install other dependencies

### Package Managers

When possible, dependencies are packaged with package managers. To install these:

```
pip install -r requirements.txt
npm install -g package.json
```

### Golang Language Server

#### Mac OS:

```
brew install gopls
```

### Magit/Forge

Set up github forge using [these instructions](https://magit.vc/manual/ghub/Getting-Started.html#Getting-Started)

### Flycut (MacOS only)

Install flycut using [these instructions](https://apps.apple.com/us/app/flycut-clipboard-manager/id442160987?mt=12).

### RustUp

```
rustup component add rust-src
```

### Ripgrep

Install ripgrep for faster search:

```
brew install ripgrep
```

### Download fonts for icons

Run command in Spacemacs:
```
all-the-icons-install-fonts
```

### Build VTerm

Install dependencies:
```
brew install cmake libtools
```
Build command (in Spacemacs):
```
vterm
```

### GDB Codesign (MacOS only)

If you would like to use GDB for debugging you will need to codesign it. This is because MacOS doesn't allow processes to access other processes for security reasons. Instructions are available [here](https://sourceware.org/gdb/wiki/PermissionsDarwin).
