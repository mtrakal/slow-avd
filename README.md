# slow-avd
How to speedup AVD android emulator

~/.android/avd/Nexus_5_API_29.avd/

edit `config.ini`

```
hw.audioInput=no
hw.audioOutput=no

hw.gps=no

hw.gpu.enabled=yes
hw.gpu.mode=host

hw.lcd.density=160
hw.lcd.height=640
hw.lcd.width=360

skin.dynamic=no
skin.path=_no_skin
skin.path.backup=_no_skin
```

In emulator: settings > Settings > Advanced:
OpenGL ES: Desktop native OpenGL
OpenGL ES API: Renderer maximum

After enable SKIA:
https://developer.android.com/studio/run/emulator-acceleration#skia-emulator
