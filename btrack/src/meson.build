add_project_arguments('-std=c++17', language: 'cpp', native: true)
add_project_arguments('-mmacosx-version-min=10.15', language: 'cpp', native: true)

eigen = dependency('eigen3')
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
executable(
    'tracker',
    src,
    include_directories: incdir,
    dependencies: eigen,
    native: true,

)
