project('crlib',
        'c')

inc = include_directories('.')

pkg_mod = import('pkgconfig')
pkg_mod.generate(libraries : crlib,
                 version : '1.0',
                 name : 'libcr',
                 filebase : 'cr',
                 description : 'A Simple C Hot Reload Header-only Library.')

install_headers('cr.h')

crlib = shared_library('foo',
                        include_directories : inc,
                        dependencies : glib_dep,
                        install : true)
