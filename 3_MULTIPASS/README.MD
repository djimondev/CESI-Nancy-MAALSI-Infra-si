# MULTIPASS

Multipass allows you to run ubuntu VM under linux / Mac / Windows.

## Introduction

Here is the [full documentation](http://multipass.run)

## To install Multipass

- [Windows](https://multipass.run/docs/installing-on-windows)
- [Linux](https://multipass.run/docs/installing-on-linux)
- [Mac](https://multipass.run/docs/installing-on-mac)

## First command lines

```
multipass --version
multipass list
watch -n 1 multipass list
multipass launch --name myvm1
multipass shell myvm1
multipass launch --name myvm2
multipass launch --name myvm3
multipass stop myvm3
multipass stop --all
multipass delete myvm1
multipass delete --all --purge
```

## To mount a volume when starting a vm

`multipass launch --name toto --mount /path-to-local-folder:/path-on-vm`

## To mount a volume on a started vm

`multipass mount /path-to-local-folder <name-of-vm>:/path-on-vm`

## To go further

```
multipass --help
multipass launch --help
```
