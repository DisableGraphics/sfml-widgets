project('sfml-widgets', 'cpp', version : '0.0.1')

sfml_dep = dependency('sfml', fallback: ['sfml', 'sfml_dep'])

sources = [
    'src/Gui/Button.cpp',
    'src/Gui/CheckBox.cpp',
    'src/Gui/Image.cpp',
    'src/Gui/Label.cpp',
    'src/Gui/Menu.cpp',
    'src/Gui/ProgressBar.cpp',
    'src/Gui/Slider.cpp',
    'src/Gui/SpriteButton.cpp',
    'src/Gui/TextBox.cpp',
    'src/Gui/Theme.cpp',
    'src/Gui/Widget.cpp',
    'src/Gui/Layouts/FormLayout.cpp',
    'src/Gui/Layouts/HBoxLayout.cpp',
    'src/Gui/Layouts/VBoxLayout.cpp',
    'src/Gui/Layouts/Layout.cpp',
    'src/Gui/Utils/Arrow.cpp',
    'src/Gui/Utils/Box.cpp',
    'src/Gui/Utils/Cross.cpp',
]

incdirs = include_directories('src/Gui')

sfml_widgets = static_library('sfml-widgets', sources, include_directories : incdirs, dependencies : [sfml_dep])

sfml_widgets_dep = declare_dependency(
   include_directories : incdirs,
   link_with : sfml_widgets,
   sources : sources)
