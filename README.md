## RIME support for Fcitx

RIME(中州韻輸入法引擎) is _mainly_ a Traditional Chinese input method engine.

[![Jenkins Build](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.fcitx-im.org%2Fjob%2Ffcitx5-rime%2F)](https://jenkins.fcitx-im.org/job/fcitx5-rime/)

[![Coverity Scan Status](https://img.shields.io/coverity/scan/13835.svg)](https://scan.coverity.com/projects/fcitx-fcitx5-rime)

tiandic 的修改版

包含如下修改:
1. 允许通过`abbrev`自定义退出ASCII模式的label提示
2. 允许自定义进入大写锁定的label提示
3. 允许自定义托盘图标(ASCII模式, 中文模式, 大写锁定模式)

注: label提示即状态切换时, 光标下的提示

### 自定义图标示例

假设自定义ASCII模式的图标为 `fc.png`

1. 在`~/.local/share/icons/hicolor/48x48/apps/`下放置`fc.png`
2. `fcitx5-configtool` -> `中州韵` -> `配置` -> `ASCII 模式图标` 填写 `fc`
