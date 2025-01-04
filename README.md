# LunarBot

A bespoke TASing bot for the NES Lunar Ball / Lunar Pool game.

It uses the [JaffarPlus](https://github.com/SergioMartin86/jaffarPlus) infrastructure.

# Requirements

```
libtbb
ncurses
openmp
meson
ninja
```

# Build

```
git clone https://github.com/SergioMartin86/LunarBot.git --recursive
mkdir build
cd build
meson .. 
ninja
```

# Usage

```
cd examples/nes/lunarBall
../../../build/lunarBot script.jaffar
```
