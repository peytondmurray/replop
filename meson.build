project(
  'replop',
  'cpp',
)

qt6 = import('qt6')
qt6_dep = dependency('qt6', modules: ['Core', 'Gui'])
inc = include_directories(

)
ui_files = qt6.compile_ui(
  sources: [
      'src/ui/mainwindow.ui'
  ]
)
# moc_files = qt6.compile_moc(
#   include_directories: inc,
#   dependencies: qt6_dep
# )
executable(
  'replop',
  'src/main.cpp',
  ui_files,
  # moc_files,
  include_directories: inc,
  dependencies : qt6_dep
)
