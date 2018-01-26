# HDF5 binaries for Trusty

This contans pre-compiled versions of HDF5 library for Ubuntu Trusty.

The best way to use these is on a case-by-case basis -- i.e. point applications that depend on HDF5 to this install location, usually via a flag like `--hdf5-lib=/path/to/hdf5_bin`.

Alternatively, you can add subdirectories of this directory to your path; e.g.

```
LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/path/to/hdf5_bin
PATH=$PATH:/path/to/hdf5_bin
export LD_LIBRARY_PATH PATH
```

To install these files to the system, clone to your machine and then copy to a directory that's in your `PATH`. **NOTE that no uninstaller is currently provided, so the only way to uninstall will be to remove these files manually.** For instance, to install to `/usr/local`:

```
sudo cp -r bin lib include /usr/local
```

To get a list of all files in this repo, you can use a command like `find . -name *`. You can then use this list to help uninstall.
