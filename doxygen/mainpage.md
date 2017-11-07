# 📚 SuperimposeMesh Library {#mainpage}

# Overview {#overview}

A modern C++ augmented-reality library to superimpose 3D objects on an images.
[TOC]


# ⚠️ About versioning {#versioning}

---
The project is undergoing _heavy_ development: APIs will be subject to changes quite often.
To be able to understand API compatibility during development, the project will follow [SemVer](http://semver.org/) specs.

In particular, the library will have **zero major version**, i.e. **0.MINOR.PATCH**, as specified by [SemVer spec. 4](http://semver.org/#spec-item-4) and the project will comply with the following rules:
 1. **MINOR** version increases when API compatibility is broken;
 2. **PATCH** version increases when functionality are added in a backwards-compatible manner;
 3. Additional labels for pre-release and build metadata are available as extensions to the 0.MINOR.PATCH format.


# 📖 Background {#background}

---
The main interest of the present library is superimposition, which refers to the placement of one thing over another so that both are still evident.
In particular, this library provides function to superimpose 3D mesh model on top of an image, which are of central importance for computer vision and augmented-reality applications.


# 🎛 Dependencies {#dependencies}

---
SuperimposeMesh library depends on
- [GLFW](http://www.glfw.org) - `version >= 3.1`
- [Open Asset Import Library, ASSIMP](http://assimp.org) - `version >= 3.0`
- [OpenGL Extension Wrangler, GLEW](http://glew.sourceforge.net) - `version >= 2.0`
- [OpenCV](http://opencv.org) - `version >= 3.0`
- [OpenGL Mathematics, GLM](http://glm.g-truc.net) - `version >= 0.9`


# 🔨 Build and link the library {#build-and-link-the-library}

---

Use the following commands to build, install and link the library.

## Build

```bash
$ git clone https://github.com/robotology/bayes-filters-lib
$ cd bayes-filters-lib
$ mkdir build && cd build
$ cmake ..
$ make
$ [sudo] make install
```

## Link

Once the library is installed, you can link it using `CMake` with as little effort as writing the following line of code in your poject `CMakeLists.txt`:
```cmake
...
find_package(SuperimposeMesh 0.MINOR.PATCH EXACT REQUIRED)
...
target_link_libraries(<target> SuperimposeMesh::SuperimposeMesh)
...
```


# 🔬 Test the library {#test-the-library}

---
We have designed some test to run with `CMake` to see whether everything run smoothly or not. Simply use
```cmake
$ ctest [-VV]
```
to run all the tests.

Tests are also a nice **starting points** to learn how to use the library and how to implement your own filters! _Just have a look at them!_


# 📘 Tutorials {#tutorials}

---
The best way to learn the basic principles about the library is by examples:
 - [Superimpose an object](@ref tutorial_superimpose)
 - [Superimpose an object with the background](@ref tutorial_superimpose_background)
