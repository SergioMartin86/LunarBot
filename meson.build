project('LunarBot','c','cpp',
  version: '3.0.0',
  license: 'GPL-3.0-only',
  default_options : ['cpp_std=c++20', 'default_library=shared', 'buildtype=release'],
  subproject_dir: 'extern'
)

# Getting current folder
srcFolder = meson.source_root()

buildLunarBallExplorer = true

## Lunar Ball Explorer (QuickerNES)

if buildLunarBallExplorer == true
jaffarSubproject = subproject('jaffarPlus', default_options : [ 'gamesFolder=' + srcFolder + '/games', 'emulator=QuickerNES'])
jaffarDependency = jaffarSubproject.get_variable('jaffarDependency')
ark1mover = executable('lunarBot',
  'games/nes/lunarBall/explorer.cpp',
  dependencies : [ jaffarDependency ]
)
endif
