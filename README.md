Dockerfiles for setting up development environments (namely CLion Toolchains). A convenience `build` script is included.

```
Usage: ./build <path to Dockerfile>

Builds an image using the Dockerfile at the specified path and tags the image
with the path. Do not include "Dockerfile" in the path.

Examples:

1) ./build actions/core # Builds a Fedora image for use with CLion
2) ./build clion/emscripten
```

The following Dockerfiles are available:

| Path | Description |
| --- | -- |
| `clion/emscripten` | Builds ontop of the Emscripten image and adds support for CLion |
| `actions/core` | Environment for GitHub Actions |