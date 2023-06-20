project('mqtt_client', 'c', 'cpp', default_options : ['c_std=c11', 'cpp_std=c++17'])

project_src = ['src/main.cpp']
db_src = ['src/db/db.cpp', 'src/db/db.hpp']
db_lib = static_library('db',db_src)

gtkdep = [dependency('gtk+-3.0'), dependency('gtksourceview-3.0')]
paho_dep = dependency('eclipse-paho-mqtt-c', method: 'cmake', modules: ['eclipse-paho-mqtt-c::paho-mqtt3c', 'eclipse-paho-mqtt-c::paho-mqtt3a'])
basic_deps = [dependency('c')]

executable('gtk-mqtt-client', project_src, link_with : db_lib,dependencies : [gtkdep, paho_dep])
