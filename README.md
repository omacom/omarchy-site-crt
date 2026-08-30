# Omarchy CRT

A CRT boot experiment, live at [crt.omarchy.org](https://crt.omarchy.org).
An old green-phosphor monitor powers on, runs POST, laser-etches the Omarchy
logo, and drops you into a terminal with the essentials from
[omarchy.org](https://omarchy.org). Press any key (or click) to boot.

Made by [Eric Carmichael](https://github.com/ckcollab)

## Running locally

The etching runs on WASM, which won't load from `file://`, so serve the folder:

```
python3 -m http.server 8765
```

Then open http://localhost:8765.

## Deploying

Pushes to `master` deploy to [crt.omarchy.org](https://crt.omarchy.org) via
GitHub Pages (see `.github/workflows/pages.yml`).
