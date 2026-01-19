# Moonforge Website

### Setting up

#### System Dependencies

Fedora:

```sh
$ sudo dnf install hugo npm
```

#### Clone

```sh
$ git clone --recurse-submodules https://github.com/moonforgelinux/moonforge-web.git
```

Or:

```sh
$ git clone https://github.com/moonforgelinux/moonforge-web.git
$ cd moonforge-web
$ git submodule update --init
```

#### Initialize

```sh
$ cd moonforge-web
$ cd themes/docsy
$ npm install
$ cd ../..
$ hugo serve
```
