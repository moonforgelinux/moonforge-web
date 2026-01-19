---
Title: 'meta-moonforge-raspberrypi'
---

# meta-moonforge-raspberrypi

This layer adds support for the Raspberry Pi 5 and 4.

#### What it does

Extends the minimal base image with recipes, distro and local configurations to build images for the Raspberry Pi.


#### How to use it

To use this layer, include the following kas file:

```yaml
header:
  version: 16
  includes:
    - kas/include/layer/meta-moonforge-raspberrypi.yml

local_conf_header:
  30_meta-moonforge-raspberrypi: |
    WKS_FILE = "moonforge-image-base-raspberrypi.wks.in"

machine: raspberrypi5
```

#### Testing

The built image can be flashed with `bmaptool`:

```
$ bmaptool copy \
> build/tmp/deploy/images/raspberrypi5/moonforge-image-minimal-raspberrypi5-0.wic.bz2 \
> /dev/sdX
```

Where `/dev/sdX` is the device of the SD card.
