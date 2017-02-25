<p align="center">
![glTF logo](https://raw.githubusercontent.com/KhronosGroup/glTF/master/specification/figures/gltf.png)
</p>

![Build Status](https://travis-ci.org/lasalvavida/COLLADA2GLTF.svg?branch=master)

# COLLADA to glTF converter

A command-line tool to convert COLLADA (`.dae`) files to [glTF](https://github.com/KhronosGroup/glTF).

## Compile from source

1. Clone repository

  ```bash
  git clone --recursive https://github.com/KhronosGroup/COLLADA2GLTF.git
  ```
2. Compile

  ```bash
  cd COLLADA2GLTF
  mkdir build
  cd build
  cmake .. && make
  ```

3. Run

  ```bash
  ./bin/collada2gltf
  ```

## Usage

```
collada2gltlf -f [file] [options]
options:
-i --input -> path of input file, argument [string]
-o --output -> path of output file argument [string]
--basePath -> resolve external uris to a different path from the input [string]
-s --separate -> output separate binary buffer, shaders and textures [bool]
-t --separateImage -> output images separately, but embed buffers and shaders [bool]
-b --binary -> output binary glTF [bool]
-m --materialsCommon -> output materials using the KHR_materials_common extension
```
