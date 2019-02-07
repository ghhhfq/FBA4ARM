
# FBA4S905&RPi-libretro
## 仅为晶晨S905、树莓派3B/3B+修改的支持更多改版游戏的FBA分支

## NEVER USE IT FOR COMMCERICAL PURPOSE.

## 严禁将本核心编译后使用在收费或者挂有募捐名义的项目中！！！


## 常见问题

### 哪里去找XXX的ROM ?
我们不提供链接，自己去搜。

### XXX游戏不能启动 ?
不是该游戏不支持，就是你的ROM有问题。先用clrmamepro重建一下ROM set吧。
有些游戏标记为不能运行，找他们的克隆ROM试试。

### XXX游戏图形有问题 ?
和上面一样，先确定你的ROM符合模拟器要求
如果问题依旧，写个带截图的报告扔给官方FBA小组吧。

### XXX游戏运行缓慢 ?
你的硬件性能不够强大，试试如下办法：
* 看看核心里有没有加速选项，有的话设为 "yes"。
* 设置跳帧。
* 在RA里关掉rewind、runahead以及任何和即时存档有关的选项。
* 在核心选项里降低声音的有关设置。
如果还是没用，升级硬件或者超频。

### XXX声音破碎 ?
原因见上一条。

### XXX游戏在MAME2003/MAME2010运行起来更快 ?
这是FBA，不是MAME，核心不同，无法相提并论。 
总之FB Alpha比旧版MAME速度慢，但是更精确，BUG更少。 
本libretro核心支持很多MAME不支持或者有BUG的功能，比如netplay、rewind、retroachievements等，这些功能会消耗一定的资源导致变慢。

### 无法使用金手指 ?
FBA本身暂不支持，但是RA支持。

### Neogeo CD游戏模拟不正常 ?
NGCD的模拟正在开发中，有些事情需要先说明一下 :
* 需要两个BIOS：neocdz.zip和neogeo.zip，分别准备好放在libretro的系统目录下。
* 需要在命令行里加上`--subsystem neocd`。
* 目前只能使用CUE+BIN或者CCD+IMG+CUE格式的镜像。
