# Crosstool-NG

## Introduction

Crosstool-NG aims at building toolchains. Toolchains are an essential component in a software development project. It will compile, assemble and link the code that is being developed. Some pieces of the toolchain will eventually end up in the resulting binaries: static libraries are but an example.

Refer to [documentation at crosstool-NG website](http://crosstool-ng.github.io/docs/) for more information on how to configure, install and use crosstool-NG.

**Note:** If you call `ct-ng --help` you will get help for `make(2)`. This is because ct-ng is in fact a `make(2)` script. There is no clean workaround for this.

## Repository layout

To clone the crosstool-NG repository:

```
git clone https://github.com/jserv/crosstool-ng
```

## Moxiebox toolchain generation

Specify moxie configurations:
```
mkdir -p ~/build-toolchain
cd ~/build-toolchain
ct-ng moxie-none-moxiebox
ct-ng build
```

After crosstool-NG builds everything from scratch, you will get GNU toolchain for Moxiebox in directory `$HOME/x-tools/moxie-none-moxiebox`.
