---
title: 設定 Mouse Button Modifier
nav_order: 7021
has_children: false
parent: 如何
---


# 設定 Mouse Button Modifier


## 說明


修改「[~/.config/openbox/bl-rc.xml](https://github.com/samwhelp/bunsenlabs-adjustment/blob/main/prototype/main/bunsen-config/Main/asset/overlay/etc/skel/.config/openbox/bl-rc.xml#L587-L614)」這個檔案

在

``` xml
  <mouse>
    <context name="Frame">

        <!-- 加入下面的「設定片段」//-->

    </context>
  </mouse>
```

將原本的「Alt」「設定片段」註解，

並且加入下面的「設定片段」

``` xml
      <!-- Window Action (Win Version) //-->
      <mousebind button="W-Left" action="Press">
        <action name="Focus"/>
        <action name="Raise"/>
      </mousebind>

      <mousebind button="W-Left" action="Drag">
        <action name="if">
          <maximized>yes</maximized>
          <then>
            <action name="UnmaximizeFull"/>
            <action name="MoveResizeTo">
              <x>center</x>
              <y>current</y>
            </action>
            <action name="Move"/>
          </then>
          <else>
            <!-- <action name="UnmaximizeFull"/> //-->
            <action name="Move"/>
          </else>
        </action>
      </mousebind>

      <mousebind button="W-Right" action="Drag">
        <!-- <action name="UnmaximizeFull"/> //-->
        <action name="Resize"/>
      </mousebind>

      <mousebind button="W-Middle" action="Click">
        <action name="Focus"/>
        <action name="Raise"/>
        <action name="ShowMenu">
          <menu>client-menu</menu>
        </action>
      </mousebind>
```


就可以[在視窗操作下面兩個動作](https://samwhelp.github.io/note-about-bunsenlabs/read/config/mousebind.html#視窗內容區塊)，

| 滑鼠按鍵組合                |  功能                   |
| --------------------------- | ----------------------- |
| `Win + [滑鼠左鍵按住拖曳]`  | 視窗移動                |
| `Win + [滑鼠右鍵按住拖曳]`  | 視窗更改大小            |




另外因為我慣用「Win鍵」的「按鍵組合」來操作一些「視窗動作」，

例如「`Win + q` => 視窗關閉」，「`Win + m` => 視窗最大化」。

預設按下「Win鍵」會觸發「顯示Menu」，

為了避免無謂的干擾，我會停用這個功能，

請參考「[停用按鍵綁定「Super_L」開啟「Menu」](https://samwhelp.github.io/note-about-bunsenlabs/read/howto/disable-keybind-open-menu.html)」這篇的說明。


## 相關議題

| 相關議題 |
| ------- |
| [滑鼠按鍵綁定](https://samwhelp.github.io/note-about-bunsenlabs/read/config/mousebind.html#視窗內容區塊) |
| [停用按鍵綁定「Super_L」開啟「Menu」](https://samwhelp.github.io/note-about-bunsenlabs/read/howto/disable-keybind-open-menu.html) |


## 相關應用

* Menu Applet 開發筆記 / [demo-mouse-button-modifier](https://samwhelp.github.io/note-about-menu-applet/read/demo/demo-mouse-button-modifier.html)
