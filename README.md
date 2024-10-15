Dockerfiles for setting up development environments (namely CLion Toolchains). A convenience `build` script is included.

```
Usage: ./build <path to Dockerfile>

Builds an image using the Dockerfile at the specified path and tags the image
with the path. Do not include "Dockerfile" in the path.

Examples:

1) ./build clion/fedora/cpp-env # Builds a Fedora image for use with CLion
2) ./build clion/emscripten
```

The following Dockerfiles are available:

| Path | Description |
| --- | -- |
| `clion/fedora/cpp-env` | Fedora environment for use with CLion |
| `clion/fedora/kokkos-libMeshb` | Builds ontop of the Fedora environment and includes Kokkos and libMeshb |
| `clion/fedora/pico-sdk` | Builds ontop of the Fedora environment and adds the pico-sdk and necessary tooling |
| `clion/emscripten` | Builds ontop of the emscripten image and adds support for CLion |
