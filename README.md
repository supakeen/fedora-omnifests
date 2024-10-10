# Fedora Omnifests

This repository is used to manage the Fedora omnifests. Omnifests are the input
format for [otk](https://github.com/osbuild/otk). `otk` compiles these omnifests
to the inputs for image build tooling.

**This repository is broken, and only an example for now.**

```
€ git clone https://github.com/supakeen/fedora-omnifests
€ cd fedora-omnifests
€ podman run -v.:/app:z ghcr.io/osbuild/otk:latest compile spin/minimal.yaml
# ... output that can be piped to `osbuild` ...
```
