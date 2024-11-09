# Fedora Omnifests

This repository is used to manage the Fedora omnifests. Omnifests are the input
format for [otk](https://github.com/osbuild/otk). `otk` compiles these omnifests
to the inputs for image build tooling.

**This repository is in rapid development, and only an example for now. Things can break at any time.**

```
€ git clone https://github.com/supakeen/fedora-omnifests
€ cd fedora-omnifests
€ podman run -v.:/app:z ghcr.io/osbuild/otk:latest compile -e environments/x86_64.yaml variants/minimal.yaml
# ... output that can be piped to `osbuild` ...
```

## `osbuild`

```
€ sudo osbuild \
    --store=/home/user/cache \
    --cache-max-size=unlimited \
    --checkpoint='*' \
    --output-directory=. \
    --export=raw \
    --export=raw-xz \
    --export=qcow2 \
    --export=tar \
    manifest.json
```

# Layout

## `/release.yaml`

## `/variants`

## `/environments`

## `/package-sets`

## `/partition-tables`

## `/library`
