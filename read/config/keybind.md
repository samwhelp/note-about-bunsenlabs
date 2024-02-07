---
title: 按鍵綁定
nav_order: 2000
has_children: false
parent: 設定
---


# 按鍵綁定


## 設定檔路徑

| 設定檔路徑 |
| ----------- |
| [~/.config/openbox/bl-rc.xml](https://github.com/samwhelp/bunsenlabs-adjustment/blob/main/prototype/main/bunsen-config/Main/asset/overlay/etc/skel/.config/openbox/bl-rc.xml#L193-L538) |
| [~/.xbindkeysrc](https://github.com/samwhelp/bunsenlabs-adjustment/blob/main/prototype/main/bunsen-config/Main/asset/overlay/etc/skel/.xbindkeysrc) |
| [~/.config/bunsen/autostart](https://github.com/samwhelp/bunsenlabs-adjustment/blob/main/prototype/main/bunsen-config/Main/asset/overlay/etc/skel/.config/bunsen/autostart#L89-L91) |




## 系統操作

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Alt + Shift + c` | Reconfigure  | `Reconfigure`       |
| `Alt + Shift + x` | Exit Dialog  | `bl-exit`           |
| `Alt + Ctrl + x`  | Openbox Exit | `Exit`              |




## 操作選單

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Alt + F1` | Root Menu | `jgmenu_run` |
| `Alt + F2` | Run Dialog | `gmrun` |




## 視窗操作

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Win + q`         | Window Close    | `Close`        |
| `Win + w`         | Window ToggleMaximize   | `ToggleMaximize`             |


| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Alt + F4`         | Window Close    | `Close`        |
| `Alt + F6`         | Window ToggleMaximize   | `ToggleMaximize`             |




## 視窗切換

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Win + a`         | Switch to Previous Window    | `PreviousWindow`        |
| `Win + s`         | Switch to Next Window    | `NextWindow`             |




## 工作空間切換

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Alt + a`         | Switch to Previous Workspace    | `GoToDesktop Previous`        |
| `Alt + s`         | Switch to Next Workspace    | `GoToDesktop Next`             |





## 視窗平鋪

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Win + Up`         | Put Window to North Side   | `Move`        |
| `Win + Down`         | Put Window to South Side    | `Move`             |
| `Win + Left`         | Put Window to West Side   | `Move`        |
| `Win + Right`         | Put Window to East Side    | `Move`             |




## 常用程式

| 按鍵組合           | 功能        | 執行指令             | 中間指令             |
| ----------------- | ------------ | ------------------- | --------------------- |
| `Alt + Enter`     | Terminal     | `lxterminal`        | `x-terminal-emulator` |
| `Alt + Shitf + a` | Terminal     | `lxterminal`        | `x-terminal-emulator` |


| 按鍵組合           | 功能        | 執行指令             | 中間指令             |
| ----------------- | ------------ | ------------------- | --------------------- |
| `Win + f`         | File Manager | `thunar`            | `bl-file-manager`     |
| `Win + b`         | Web Browser  | `firefox`           | `x-www-browser`       |
| `Win + e`         | Text Editor  | `geany`             | `bl-text-editor`      |
| `Win + t`         | Terminal     | `lxterminal`        | `x-terminal-emulator` |


| 按鍵組合           | 功能        | 執行指令             | 中間指令             |
| ----------------- | -------------- | ------------------- | --------------------- |
| `Win + m`         | Media Player   | `vlc`               | `bl-media-player`     |
| `Win + v`         | Volume Control | `pavucontrol`       |                       |
| `Win + h`         | Task Manager   | `htop`              |                       |


| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | --------------------- |
| `Win + l`         | Lock Screen  | `bl-lock`             |
| `Win + x`         | Logout       | `bl-exit`             |
| `PrtSc`           | Screenshot   | `xfce4-screenshooter` |
