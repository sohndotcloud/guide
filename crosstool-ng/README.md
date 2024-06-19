# Crosstool-NG - Fedora 40

### Installation steps:

Pull down the latest project from **`git clone https://github.com/crosstool-ng/crosstool-ng`** to grab a copy of the **source**

*Before the project is built, the project templates need to compile first.*

**Run `./bootstrap`**

**Run `$CROSSTOOL-NG_DIR/install_fedora_dep.sh`**

The **prefix field** of the configure script is the target output directory.

```
./configure --prefix=/app/dir/path
make
make install
```

The source project can be deleted.

The executable can be added to $PATH to be callable from bash.

`export PATH="/app/dir/path/bin/:$PATH"`

or copy the bin to the local user bin folder under $PATH.

`cp /app/dir/path/bin/ct-ng /home/.local/bin`




## REFERENCE
https://crosstool-ng.github.io/docs/install/