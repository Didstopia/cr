project('cr', 'c')

inc = include_directories('.')

install_headers('cr.h')

cr = library(
    'cr',
    include_directories: inc,
)

cr_dep = declare_dependency(
    link_with: cr,
    include_directories: inc,
)
