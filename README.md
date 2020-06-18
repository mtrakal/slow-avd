# How to speedup AVD android emulator
https://developer.android.com/studio/releases/emulator

## Enable virtualization: 
https://developer.android.com/studio/run/emulator-acceleration#accel-vm

~/.android/avd/Nexus_5_API_29.avd/

edit `config.ini`

```
hw.accelerometer=false

hw.audioInput=no
hw.audioOutput=no

hw.gps=no

hw.gpu.enabled=yes
hw.gpu.mode=host

hw.lcd.density=160
hw.lcd.height=640
hw.lcd.width=360

hw.sensors.proximity=false

skin.dynamic=no
skin.path=_no_skin
skin.path.backup=_no_skin
```

In emulator: settings > Settings > Advanced:
```
OpenGL ES: Desktop native OpenGL
OpenGL ES API: Renderer maximum
```

### After enable SKIA:
https://developer.android.com/studio/run/emulator-acceleration#skia-emulator


## How to enable Google Play in custom emulator:
```
PlayStore.enabled=true
image.sysdir.1=system-images\android-29\google_apis_playstore\x86\
tag.display=Google Play
tag.id=google_apis_playstore
```
