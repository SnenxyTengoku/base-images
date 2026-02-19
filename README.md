# Base images &nbsp; [![bluebuild build badge](https://github.com/snenxytengoku/base-images/actions/workflows/build.yml/badge.svg)](https://github.com/snenxytengoku/base-images/actions/workflows/build.yml)

Base images, made to be a minimal base for others to use to build their own images. Should be self-maintained and always up-to-date.

Usually, images here are forked or "inspired" off of other's work, but modified to fit better/more customizable needs.

Won't include everything, obviously. Look at [BlueBuild's](https://github.com/blue-build/base-images) and [Universal Blue's](https://github.com/ublue-os/main) bases for more usable templates.

There's no goals for these images, other than attempting to strike a good middle ground between staying "minimal enough", but not "include literally nothing" for builders to struggle with.
- These images mainly focus *desktop* usage;
- *Will* include uBlue/BlueBuild default changes.

Refer to [BlueBuild](https://blue-build.org)'s documentation for more information.

## `niri`

Fedora image with [niri](https://github.com/niri-wm/niri) included, and a few extras. "Inspired" by [Wayblue](https://github.com/wayblueorg/wayblue)'s `niri` image, but with less additions and clean-up/modernization of some modules. <small>*Lots* of homework copied from them, so props to the Wayblue team.</small>

- Use Universal Blue's `base-main` as base image
- Minimize script usage/custom additions
- Includes [xwayland-satellite](https://github.com/Supreeeme/xwayland-satellite)
- Don't preinstall custom utilities (e.g. terminal, bar, launchers, notification manager, etc.; The builder *is* expected to extend with their preferred applications and configurations, anyways)

## `mangowc`

Fedora image with [MangoWC](https://github.com/DreamMaoMao/mangowc) included, and the extra basics.

- Use Universal Blue's `base-main` as base image
- Includes `xorg-xwayland`

## Other images

### `kutia`

A "mainly for custom use, unless you have a usecase for this too" image that merges both `niri` and `mangowc` into one, including both window managers and utilities into one image.
