project('tutorial', 'c', 'cpp',
default_options : ['c_std=c11', 'cpp_std=c++17'])
project_src = ['src/main.cpp']
gtkdep = [dependency('gtk+-3.0'), dependency('gtksourceview-3.0')]
executable('gtk-mqtt-client', project_src, dependencies : gtkdep)
