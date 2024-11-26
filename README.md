# GLFW precompiled shared library
This project holds the precompiled GLFW3 library along with the include directory extracted from the ubuntu packages
`libglfw3` and `libglfw3-dev` found [here](https://packages.ubuntu.com/jammy/libglfw3) and [here](https://packages.ubuntu.com/oracular/libglfw3-dev).

## Build

### Meson
Add the following `glfw3.wrap` file to your `subprojects` directory:
```
[wrap-git]
url = git@github.com:makredzic/glfw.git
revision = HEAD
```

In the **project root** meson build file, you can now simply use `dependency('glfw3')` to fetch the `glfw` dependency.
