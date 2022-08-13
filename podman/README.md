# Build a deb package from PKGBUILD

```
# build makedeb image
$ podman build --layers=false --tag makedeb .

# compile deb package
$ podman run --rm -v <DIR_CONTAINING_PKGBUILD_FILE>:/makedeb localhost/makedeb
```
