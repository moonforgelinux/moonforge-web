---
Title: 'Build'
---

# Build

The `build` configuration fragment 

### What it does

- Sets up the Hash Equivalence server from the host
- Makes sure builds use only cached sources

### Example

You can use the `build` fragment with `kas`:

```sh
$ kas-container build kas/examples/moonforge-image-base-raspberrypi5.yml:kas/common/build.yml 
```
