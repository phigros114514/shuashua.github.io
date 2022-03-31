# [Demo](https://lch&#122;h&#51;473.github.io/canvas/phi/index "Phigros模拟器")

## 简介

如题，用js/canvas还原Phigros游戏画面，属于个人兴趣项目，仅用于学习和测试；

模拟器代码部分为作者独立编写，与《Phigros》游戏本体无关，您因使用或修改代码所造成的一切后果由您自己承担；

不提供游戏本体安装包及逆向工具/教程，也不提供谱面下载；

模拟器并不拥有官方素材(如音符贴图/打击音效/结算UI)的版权，如有侵权请联系模拟器作者下架相关内容。

感谢[@Mac-Fus](https://space.bilibili.com/319384496)提供虚拟机支持

感谢[@星星awa](https://space.bilibili.com/111933676)提供Safari适配思路

## 更新日志

### [1.4.15] - 2022.3.31

#### 新内容

* 新增pec谱面`Note`方向数值检测
* ~~没有别的更新了qwq~~

#### 修复

* 修复了部分包含时间异常事件的谱面不正常显示的bug

#### 已删除

* 移除HyperMode

### [1.4.14] - 2021-12-23

#### 新内容

* 新增功能：`谱面镜像`(实时生效)
* 新增功能：`音乐变速`(非实时生效，启用时无法存档)
* 新增Early/Late特效复选框(测试功能)

#### 更改

* 现在`信息`选项卡无信息时会显示一条文案

### [1.4.13] - 2021-11-22

#### 新内容

* ~~新增HyperMode：更加严格的判定和结算(测试功能)~~
* ~~新增Great判定：40-80ms(显示为绿色特效，HyperMode特有)~~
* 新增Early/Late统计(结算界面点击切换)

#### 更改

* 针对低帧率画面调整打击判定，提升稳定性
* 暂停时点击画面不再触发打击判定

#### 修复

* 修复了部分设备非全屏触摸点向上错位的bug

### [1.4.12] - 2021-11-15

#### 新内容

* 新增zip模块兼容性检测(测试功能)

#### 修复

* 修复了画面高度小于一定值时全屏触摸点向下错位的bug
* 修复了pec谱面结尾的n指令无法正常读取的bug

#### 已删除

* 移除可选链操作符和WebAssembly兼容性检测
* 移除视频录制功能

### [1.4.11] - 2021-10-23

#### 新内容

* 新增pec谱面事件时间检测(测试功能)

#### 更改

* 为`Hold`添加多押高亮(与官方v2.0.0一致)

#### 修复

* 修复了画面高度大于一定值时部分`Note`无法正常显示的bug
* ~~修复了pec谱面结尾的n指令无法正常读取的bug~~

### [1.4.10] - 2021-10-10

#### 更改

* 画面左上角播放进度：暂停时会显示`(Paused)`

#### 修复

* 修复了`info.csv`配置不当导致谱面显示错误的bug
* 修复了进入结算界面之前重新开始仍会结算的bug

### [1.4.9] - 2021-10-03

#### 更改

* 画面左上角播放进度：当分钟小于10时不再补0

#### 修复

* 修复了因上版本播放逻辑造成音频撕裂的bug(将播放逻辑回退至1.4.7)
* 修复了过渡动画结束前判定时间内的`Note`可以被打击的bug
* ~~修复了进入结算界面之前重新开始仍会结算的bug~~

### [1.4.8] - 2021-09-21

#### 优化

* ~~优化音频播放逻辑，使音频与谱面保持同步~~

#### 修复

* ~~修复了过渡动画结束前判定时间内的`Note`可以被打击的bug~~
* ~~修复了进入结算界面之前重新开始仍会结算的bug~~
* 修复了部分不支持视频录制的浏览器无法使用模拟器的bug

### [1.4.7] - 2021-09-20

#### 新内容

* 新增浏览器兼容性检测(测试功能)
* 新增pec谱面异常`Note`和负数`Alpha`检测(测试功能)

#### 优化

* 为iPhone全面屏提供适配

### [1.4.6] - 2021-09-15

#### 新内容

* 隐藏文件：zip内包含以`.`开头的文件将被隐藏，不会显示在选项框

#### 优化

* 优化图像和字体渲染
* 为Safari浏览器适配全屏功能

#### 更改

* `Hold`连续打击特效间隔现在与判定线`bpm`成反比
* `Autoplay`开启时，结算画面不再显示"+0"
* 产生Bad判定的`Note`现在会跟随判定线
* pec谱面默认偏移由-150ms改为-175ms

### [1.4.5] - 2021-09-10

#### 新内容

* 新增键盘操作，感受极其生草的游戏体验(测试功能)

#### 优化

* 为Safari浏览器适配离屏自动暂停功能

#### 更改

* 若Bad判定范围内的`Tap`前方存在未打击的`Drag`或`Flick`将不触发Bad判定
* 暂停快捷键由`Space`(空格)改为`Shift`(左右Shift均可)
* 调整了结算界面`AUTO PLAY`的显示位置

### [1.4.4] - 2021-09-09

#### 新内容

* 新增`触摸反馈`和`背景模糊`复选框(实时生效)
* 新增本地存档(仅在关闭`Autoplay`并开启`过渡动画`时存档)

#### 优化

* 对Safari浏览器进行部分适配
* 优化文件读取逻辑，现在能够支持更多文件类型
* 优化图像渲染

#### 更改

* 结算界面背景音乐会随等级变化(仅在进入结算界面前生效)

### [1.4.3] - 2021-09-02

#### 新内容

* 新增功能：`谱面延时`(非实时生效)
* 添加防止模拟器泛滥的提示
* 新增错误提示(现在导入不包含音乐的zip文件也会报错)

#### 优化

* 优化页面布局

#### 更改

* `Hold`渲染由倒序改为顺序(其余`Note`渲染顺序仍为倒序)
* 导入zip：背景图片由必需改为可选(无图片时将替换为纯白背景)
* 过渡动画由逐帧控制改为计时器控制

#### 修复

* 修复了过渡开始动画判定线颜色不随`FC/AP指示器`变化的bug

### [1.4.2] - 2021-09-01

#### 更改

* 双击判定区域由圆形改为矩形

#### 修复

* 修复了无法判定`HoldTime`小于0.2s的`Hold`的bug

### [1.4.1] - 2021-09-01

#### 新内容

* 新增画面双击判定：左上角暂停，右上角重新开始

#### 优化

* 优化触摸点定位逻辑

#### 更改

* 增大画面双击判定范围(现在与画面文字大小成正比)

#### 修复

* 修复了开启`显示定位点`时无法统计note数目的bug
* 修复了逐帧判定导致严重吃音的bug
* 修复了结算界面"φ"评级有几率错误地显示为“V”的bug

### [1.4] - 2021-08-31

#### 新内容

* 新增`FC/AP指示器`复选框(实时生效)
* 新增游玩模式(测试功能，需关闭`Autoplay`复选框)
* 新增结算界面(测试功能，在歌曲结束后出现，需开启`过渡动画`复选框)
* 新增错误提示(导入非zip文件或不包含谱面的zip文件均会报错)

#### 优化

* 优化图片颜色渲染机制

#### 更改

* 打击特效动画更加接近官方(1.6.11)
* 单个打击特效时长由30tick改为500ms
* 切换全屏的方式改为双击画面右下角

#### 修复

* 修复了关于pec谱面第一个bp指令延时不为0导致谱面错误偏移的bug

### [1.3.2] - 2021-08-16

#### 优化

* 优化绘制逻辑，提升性能

#### 修复

* 修复无判定线事件的谱面无法播放的问题

#### 更改

* `Note`定位文字改为`判定线序号±Note序号`(例如0号判定线上方的第0个Note定位文字为`0+0`)

### [1.3.1] - 2021-08-11

#### 新内容

* 新增功能：视频录制(测试功能，录制时无法暂停)

#### 更改

* 实装`info.csv`和`line.csv`，简介新增悬浮提示
* 连击字样`combo`改为`Autoplay`
* `显示定位点`功能：画面左下角显示不同种类已打击`Note`的实时数量，负数`Note`以半透明显示

### [1.3] - 2021-07-11

#### 新内容

* 对pec谱面的bpm变速功能进行适配
* 新增功能：过渡动画(包含开头淡入和结尾淡出，不包含结算)
* 新增输入框(曲绘、谱师)，对应过渡动画
* 通过添加`line.csv`以修改判定线贴图(测试功能)
* 通过添加`info.csv`以自动填写谱面信息(测试功能)

#### 优化

* 优化zip文件读取逻辑(数组→对象)
* 优化判定线和背景的绘制顺序
* 调整背景和UI对不同尺寸屏幕的适配
* 打击特效动画采用缓动函数
* 调整打击音效与官方v1.6.10一致
* 优化`播放/停止`和`暂停/继续`按钮相关逻辑

#### 更改

* `宽高比`下拉列表新增`10:7`(适配iPad Pro 11)，将`256:175`改为`19:13`(适配Phi Editor)
* `显示定位点`功能：判定线数字透明度随判定线透明度变化，`Note`打击后变为半透明
* `Hold`尾判调整为提前0.2秒得分
* `Hold`连续打击特效间隔由12tick缩短为9tick

#### 修复

* 修复了部分谱面`Note`打击时间异常的bug
* 修复了有关pec谱面判定线事件time不精确导致排序错误的bug
* 修复了点击`停止`按钮后按住的`Hold`无法关闭导致连击得分溢出的bug

### [1.2.2] - 2021-07-03

#### 新内容

* `显示定位点`现在能对`Note`进行定位(测试功能)

#### 修复

* 修复包含文件夹的zip无法正确加载的问题
* 修复了部分谱面`Note`速度异常及`Hold`错位的bug

#### 更改

* 谱面默认速度：`1.0`→`1.2`(json)，`1/5.75`→`1/7.0`(pec)
* 打击特效颜色：`#fce491`(Perfect)，`#9ed5f3`(Good)

### [1.2.1] - 2021-06-22

#### 新内容

* 添加下拉列表(宽高比、按键缩放、背景变暗)
* 对pec谱面的`Fake Note`进行适配(测试功能)

#### 修复

* 修复了有关pec判定线演出的若干bug

### [1.2] - 2021-06-12

#### 新内容

* 支持导入pec(暂未适配`Fake Note`和`Alpha值扩展`)

### [1.1] - 2021-05-04

#### 新内容

* 支持导入zip、选择谱面及一些基本操作

#### 已删除

* 暂时移除`模拟Demo`

### [1.0.1] - 2021-04-18

#### 更改

* `模拟Demo`改为Phigros愚人节谱`Spasmodic SP`

### [1.0] - 2021-01-28
