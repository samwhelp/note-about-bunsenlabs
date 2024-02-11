---
title: 停用按鍵綁定「Super_L」開啟「Menu」
nav_order: 7022
has_children: false
parent: 如何
---


# 停用按鍵綁定「Super_L」開啟「Menu」


## 設定檔路徑

| 設定檔路徑 |
| ----------- |
| [~/.config/bunsen/autostart](https://github.com/samwhelp/bunsenlabs-adjustment/blob/main/prototype/main/bunsen-config/Main/asset/overlay/etc/skel/.config/bunsen/autostart#L89-L91) |
| [~/.xbindkeysrc](https://github.com/samwhelp/bunsenlabs-adjustment/blob/main/prototype/main/bunsen-config/Main/asset/overlay/etc/skel/.xbindkeysrc#L57-L59) |



## 說明


原本「Bunsenlabs」在「[~/.xbindkeysrc](https://github.com/samwhelp/bunsenlabs-adjustment/blob/main/prototype/main/bunsen-config/Main/asset/overlay/etc/skel/.xbindkeysrc#L57-L59)」這個檔案，

有做了一個「按鍵綁定」，設定片段如下：

```
# Show main menu
"jgmenu_run"
    Mod4 + space
```

也就是當按下了「`Win + Space`」，就會執行「`jgmenu_run`」。

也就是啟動「開始功能表」。


另外可以在「[~/.config/bunsen/autostart](https://github.com/samwhelp/bunsenlabs-adjustment/blob/main/prototype/main/bunsen-config/Main/asset/overlay/etc/skel/.config/bunsen/autostart#L89-L91)」這個檔案，

可以看到一個按鍵映射設定，設定片段如下：

``` sh
    ## Alias Super key to Super+Space for single-key menu.
    ## See 'man xcape' for other possibilities.
    xcape -e 'Super_L=Super_L|space'
```

也就是當按下了「`Win`」就會映射到「`Win + Space`」，

接著就會啟動「開始功能表」。

所以我們要**停用按鍵綁定「Super_L」開啟「Menu」**

只要將「`xcape -e 'Super_L=Super_L|space'`」這一行註解就行了，

也就是將剛剛上面的那個設定片段，改成如下：

``` sh
    ## Alias Super key to Super+Space for single-key menu.
    ## See 'man xcape' for other possibilities.
    #xcape -e 'Super_L=Super_L|space'
```




## 相關議題

| 相關議題 |
| ------- |
| [設定 Mouse Button Modifier](https://samwhelp.github.io/note-about-bunsenlabs/read/howto/config-mouse-button-modifier.html) |
