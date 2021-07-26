---
title: 魔兽字体修改
layout: post
post-image: "https://raw.githubusercontent.com/thedevslot/WhatATheme/master/assets/images/What%20is%20Jekyll%20and%20How%20to%20use%20it.png?token=AHMQUELVG36IDSA4SZEZ5P26Z64IW"
description: Jekyll is a static site generator. You give it text written in your favorite
  markup language and it uses layouts to create a static website.
tags:
- 插件
- 界面

---

修改方法，将字体放置于魔兽世界根目录下的 Fonts 文件夹下，重启游戏即可，字体必须为 TrueType 格式，后缀为ttf。

Bash 下用于自动修改字体的脚本：

> # `#!/bin/bash

set -e

cd "${0%/*}"

UI_FONT=_ui_font.ttf
CT_FONT=_ui_font.ttf

# English
# cp $UI_FONT ARIALN.TTF # chat, info text, small text
# cp $UI_FONT FRIZQT__.TTF # main UI font, INCLUDES combat text
# cp $UI_FONT MORPHEUS.TTF # mail text, quest log header text
# cp $CT_FONT SKURRI.TTF # unit frame combat text

# Chinese Simplified
cp $UI_FONT ARHei.TTF # item, spell description
cp $UI_FONT ARKai_T.TTF # main UI font
# cp $CT_FONT ARKai_C.TTF # Combat text

echo -e "Done! you can close this window now."`
