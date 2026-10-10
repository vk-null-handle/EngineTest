# Elysian Game Engine

This is a simple 3d only game engine written from the ground up using C99, made to learn the Vulkan graphics API, linear maths, and game engine design.
It is currently **not production-ready** as it is lacking most features of, well a game engine. However, this will change in the future.

## Current features:
- Clang and GCC support
- Renderer with a modern Vulkan 1.4 backed made using latest features and techniques
- Project generation (See other branch)

## Platform & compiler support:
Currently only Clang and GCC are supported, MSVC is untested.
The project is being developed on Arch linux (btw), but uses GLFW for platform abstraction so it could be built on windows.

## Prerequisites:
Since this engine is made as a learning experience almost everything is made from scratch where possible, so there are minimal 3rd party dependencies. However, to build it you will need:
- [Vulkan SDK](https://vulkan.lunarg.com/) (version 1.4 minimum)
- Either [GCC](https://gcc.gnu.org/releases.html) or Clang
- [GLFW](https://www.glfw.org/download)
- [Shaderc](https://github.com/google/shaderc)

## Building

**Clone the repository:**
```
git clone https://github.com/vk-null-handle/elysian
```

**Run make to build project:**\
By default it will try to compile with Clang, but you can change the CC variable at the top to GCC if needed.
```
make
```

**Run:**\
Currently ./testbed is the engine running application, but in the future there will be user created projects and an editor.
```
make run
```

**Generate compile commands with:**
```
bear -- make rebuild
```

## License:
This project is licensed under the MIT license see more details in the [LICENSE.txt](./LICENSE)
