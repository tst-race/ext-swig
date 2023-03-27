# SWIG for RACE

This repo provides scripts to custom-build the
[SWIG tool](https://www.swig.org/) for RACE.

## License

The SWIG tool is licensed under the GPL license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

SWIG has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build SWIG.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-swig.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-swig
```

## Platforms

SWIG is built for the following platforms:

* `linux-x86_64`
* `linux-arm64-v8a`

## How It Is Used

SWIG is used directly by the RACE core.
