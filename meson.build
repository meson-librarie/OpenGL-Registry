project('opengl-registry', ['c'],   
         meson_version : '>= 0.49.0')




egl_registry_project = subproject('egl-registry')
egl_registry_dep = egl_registry_project.get_variable('egl_registry_dep')




opengl_registry_dep = declare_dependency(
  include_directories: include_directories('api'),
  dependencies: [egl_registry_dep]
)




install_subdir('api', install_dir : 'include', strip_directory : true)