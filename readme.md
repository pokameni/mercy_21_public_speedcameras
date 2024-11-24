# 🛰️ Mercy_21's Public Speed Cameras — v1.0
- Topic Link : https://forum.cfx.re/t/free-speed-camera-hacking-wip/5270153
### 📹 Previews
- https://streamable.com/9xnkmv

### ⭐ Features
- This script adds a speed camera system with fining enabled by default.
- This script also adds an option to disable them through `bl_ui` minigames.
- In roleplay terms, you'll send a virus on a satellite, with some physical access points around LS.

### 📃 You'll need this :
- [ox_lib](https://github.com/overextended/ox_lib/releases/latest)
- [bl_ui](https://github.com/Byte-Labs-Studio/bl_ui)
- qbCore

### 👨🏻‍💻 How to install
- Download our source code / latest release.
- Put it on your server.
- Put the resource name on your `server.cfg` or `resources.cfg` file

### 👨🏻‍💻 How to configure
- You can edit in-game messages in lines 73, 134, 181, 196, 205, 214 of the `disablecam.lua`.
- Sending virus will only work if user won one of them randomly picked `bl_ui` minigames.
```lua
local minigames = {-- in the disablecam.lua
    function() return exports['bl_ui']:CircleProgress(1, 50) end,
    function() return exports['bl_ui']:Progress(1, 50) end,
    function() return exports['bl_ui']:KeySpam(1, 50) end,
    function() return exports['bl_ui']:KeyCircle(1, 50, 3) end,
    function() return exports['bl_ui']:NumberSlide(1, 50, 3) end,
    function() return exports['bl_ui']:RapidLines(1, 50, 5) end,
    function() return exports['bl_ui']:CircleShake(1, 50, 3) end
}
```

Physical access points for sending viruses to satellite :
```lua
local satellitePoints = { -- in the disablecam.lua
    vector3(213.05, -998.62, 28.29),
    vector3(-144.89, -419.76, 33.39),
    vector3(-803.76, -96.02, 36.59),
    vector3(-1087.07, -1325.5, 4.23),
    vector3(731.56, 146.07, 79.75),
    vector3(297.39, -355.49, 44.15),
    vector3(-22.57, 45.98, 71.24),
    vector3(-1443.39, -782.83, 22.47),
    vector3(-968.66, -177.75, 36.8),
    vector3(-911.98, -100.89, 37.23),
    vector3(-1008.41, 303.83, 67.07),
    vector3(-468.56, -722.48, 31.73),
    vector3(13.7, -790.34, 30.77),
    vector3(109.42, -820.83, 30.31)
}
```

### Credits :
- mercy_public / turtle8675309 (actual script)
- P4NDAzzGaming (Origian Creator of [esx_speedcameras](https://github.com/P4NDAzzGaming/esx_speedcamera))
- Tom Osborne (Creator of [qb-speedcameras](https://github.com/tom-osborne/qb-speedcameras))
