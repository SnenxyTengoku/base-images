# Base images &nbsp; [![bluebuild build badge](https://github.com/snenxytengoku/base-images/actions/workflows/build.yml/badge.svg)](https://github.com/snenxytengoku/base-images/actions/workflows/build.yml)

> [!NOTE]
> This repository is currently unused. No images yet exist.

Base images, made to be a minimal base for others to use. Should be self-maintained and always up-to-date.

Usually, images here are forked off other's worked but modified to fit better/more customizable needs.

Refer to [BlueBuild](https://blue-build.org)'s documentation for more information.

## `niri`

Fedora image with niri included, and a few extras. Forked off of [Wayblue](https://github.com/wayblueorg/wayblue)'s `niri` image, but with less additions and clean-up/modernization of some modules.

- Use `quay.io/fedora/fedora-bootc` as base image
- Use `dnf` instead of `rpm-ostree`
- Minimize script usage/additions, namely don't remove "unused repositories" (Universal Blue conversion still included)
- Don't preinstall custom utilities (e.g. notification manager, bar, etc.; The builder *is* expected to extend with their preferred applications, anyways)