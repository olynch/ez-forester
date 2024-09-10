# EZ-Forester

This is a script that you can place in your forest repository that downloads and runs forester, so that instead of installing opam/nix, someone can get started with forester by simply running.

```bash
./forester build
```

Behind the scenes, it downloads and caches a binary to ~/.forester/VERSION. Supported operating systems/architectures include macOS (intel and ARM), and linux (intel).

To install this in your repository, simply copy "forester" and "checksums.txt" into your repository, and update the "VERSION" variable when you want to upgrade forester. I (Owen) will try to keep the binary builds up to date, though I may lag behind when new releases come out.

Of course, this relies on you trusting that I haven't done anything funny with the binaries that are being downloaded. If you value security over convenience, then I encourage you to build your own forester, which is really not too hard, and can be done with either opam or nix.
