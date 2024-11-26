project(
  'glfw',
  'cpp',
  version: '3.3.6-1'
)

cpp = meson.get_compiler('cpp')

glfw_lib = cpp.find_library('glfw', dirs: meson.current_source_dir() + '/lib')
glfw_hdr = include_directories('include')

glfw_dep = declare_dependency(
  dependencies: glfw_lib,
  include_directories: glfw_hdr,
)

meson.override_dependency('glfw', glfw_dep)


