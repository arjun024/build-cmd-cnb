# build-cmd-cnb

Executes an arbitrary file named `build_cmd.sh` (if present) at the root of the
app during the build phase.

Building
========

jam pack --buildpack buildpack.toml --version 1.0.0 --output build-cmd-cnb.tgz

Needs [jam](https://github.com/paketo-buildpacks/packit/releases)


Example
======

See [example](./example)

```
pack build testapp -p example -b build-cmd-cnb.tgz

docker run testapp /workspace/hello
```

Needs [pack](https://github.com/buildpacks/pack/releases)
