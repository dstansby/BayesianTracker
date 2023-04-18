cpp = meson.get_compiler('cpp')
add_project_arguments('-std=c++17', language: 'cpp', native: true)

if cpp.get_id() == 'clang'
    add_project_arguments('-mmacosx-version-min=10.15', language: 'cpp', native: true)
endif

incdir = include_directories('../include')
src = [
    'bayes.cc',
    'hyperbin.cc',
    'hypothesis.cc',
    'interface.cc',
    'manager.cc',
    'motion.cc',
    'pdf.cc',
    'tracker.cc',
    'tracklet.cc',
    'wrapper.cc',
]
library(
    'libtracker',
    src,
    include_directories: incdir,
    dependencies: eigen,
    native: true,
    install: true,
)
