# 配置详情 v1

- 配置信息存储在同级目录的 `InputTip.ini` 文件中，启动软件时自动创建
  - 如果 v1 v2 版本都使用过，不用担心，它们的配置信息是独立的，不会冲突
- 修改方式:
  - 鼠标右键点击任务栏右侧的 `InputTip.exe` 图标，点击 `更改配置`。(推荐方式)
  - 直接打开 `InputTip.ini` 文件，修改对应项的值，保存后重启 `InputTip.exe`。

---

## `font_family`

- 默认值: `SimHei`
- 指定显示的字体

## `font_size`

- 默认值: `12`
- 字体大小(显示大小)

### `font_weight`

- 默认值: `900`
- 字体粗细

### `font_color`

- 默认值: `ffffff`
- 字体颜色
- 可以是常见的颜色英文名，也可以是十六进制颜色值(带不带 `#` 都可以)。

### `font_bgcolor`

- 默认值: `474E68`
- 背景颜色
- 可以是常见的颜色英文名，也可以是十六进制颜色值(带不带 `#` 都可以)。

### `windowTransparent`

- 默认值: `222`
- 透明度。
- 取值范围: `0`~`255`

### `CN_Text`

- 默认值: `中`
- 中文状态显示的字符

### `EN_Text`

- 默认值: `英`
- 英文状态显示的字符

### `Caps_Text`

- 默认值: `Caps`
- 大写锁定状态显示的字符

### `offset_x`

- 默认值: `30`
- 显示位置的水平偏移量

### `offset_y`

- 默认值: `-50`
- 显示位置的垂直偏移量

### `window_no_display`

- 默认值: `notepad.exe,everything.exe`
- 这里需要一个列表(以英文逗号 `,` 分隔)，如果打开的程序在这个列表里，则当输入法中英文切换时，不会显示对应的方块符号
  - 因为在一些程序中，无法获取到输入法中英文状态，对于这些程序，就应该让它隐藏方块符号，只让它在大写锁定状态下显示
  - 默认值中的 `notepad.exe` 和 `everything.exe` 这两个程序，就无法获取到输入法中英文状态，索性就就当默认值了