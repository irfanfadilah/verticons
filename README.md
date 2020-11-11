# Verticons
Simple Rainmeter Skin for Displaying Icons/Shortcuts Vertically 

# Screenshot

![ScreenShot](https://user-images.githubusercontent.com/6077598/98790285-112e1a00-2436-11eb-9d0a-9fee0e8afeda.png)

# Download

[Verticons_1.0.rmskin](https://github.com/irfanfadilah/verticons/releases/download/1.0/Verticons_1.0.rmskin) (28.2 KB)

# Adding Icon

You can use this template below or copy-paste from existing entries in `Icons.ini`:

```
[ICON_NAME]
Meter=Image
W=#IconSize#
H=#IconSize#
X=#BasePosition#
Y=(#BasePosition# + #IconDistance# * X)
SolidColor=0,0,0,1
ImageName=assets/ICON_IMAGE.png
LeftMouseUpAction=["C:\Program Files\SOMETHING\SOMETHING.exe"]
```

Replace the `X` with (icon position - 1). So if it's your 6th icon in the entries, the X would be 5.

Replace `ICON_NAME`, `ICON_IMAGE.png` and `Target PATH` accordingly.

All the icons are placed under `Verticons/Icons/assets`.

# Variables

`IconSize` => Icon size in pixel.

`IconDistance` => Distance between icons in pixel.

# Icon Transparency

I don't want to set the transpareancy in the Meter, you can adjust it manually, e.g.: `Settings > Transparency > 30%`.

# Where to Get More Icons?

You can use your favorite icon packs, but in this skin I'm using the icons from https://remixicon.com/.

If you need white colored icons, you can download and edit (invert) it by yourself in an image editor like GIMP.

# Horizontal Version?

You can just swap the `X` and `Y` of each entries, e.g.:

```
[Icon]
xxxxxxxxxx
xxxxxxxxxxxx
xxxxxxxxxxxxxx
X=#BasePosition#
Y=(#BasePosition# + #IconDistance# * 3)
xxxxxxxxxxxxxxxxxxxx
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

to:

```
[Icon]
xxxxxxxxxx
xxxxxxxxxxxx
xxxxxxxxxxxxxx
X=(#BasePosition# + #IconDistance# * 3)
Y=#BasePosition#
xxxxxxxxxxxxxxxxxxxx
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

# License

WTFPL
