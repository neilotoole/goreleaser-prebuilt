# GoReleaser Pro Prebuilt Example

This repo contains a quick and to-the-point example of how to use
[GoReleaser Pro](https://goreleaser.com/pro)
[prebuilt builder](https://goreleaser.com/customization/build/#import-pre-built-binaries).

To run it, clone this repo and run:

```sh
goreleaser release --snapshot -f 1.yml
```

This will create the binaries in `/tmp/dist`.

Next, run:

```sh
goreleaser release --snapshot -f 2.yml
```

This will import the binaries and create archives, nfpm packages, etc.

The `--snapshot` flag is optional in the "real world".
It is required here because its just an example.
