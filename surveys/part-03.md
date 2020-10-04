# RenPy
> RenPy定制了一套脚本语言，后缀为`.rpy`；脚本中同时包含了背景，音乐，对话，变量声明，逻辑控制流……即脚本就是游戏的完整定义
> （这和我未实现的[想法](https://github.com/iamhyc/Bard-Engine)是完全一致的，我只是缺少了开发脚本引擎的能力，以及当时想一步到位开发物理引擎，起步点太高；不过既然有RenPy了，我就只需要专心于NLP翻译就好了）

- audio / images 文件夹是默认的音频/图像文件夹，其中 images 包含了 `Movie`tag 的创建，audio则包含了人物语音
> 这是不好的，在 Bard Engine 设计中要对不同的资源（SE, BGM, BG, CG, etc.）做区分
- `script.rpy`中就是脚本的全部了，没必要去调整 `gui.rpy/options.rpy/screens.rpy` 这些和发行相关的内容
- `image`的名字由空格分隔，第一个是图片的tag名称（标识后续相同tag的更新），后面的是图片的属性；虽然这并没有什么用呵呵
- `narrator`是特殊的Character，默认不带发言人的就是narrator
- RenPy支持[组合图像资源](https://www.renpy.cn/doc/layeredimage.html)，可以用在资源自动生成上
- 支持[Ruby文体](Ruby文本(较常用来标明假名或者注音)是一种在某个字符或单词上方显示小号文本的文本)，可以考虑下加在script支持里（注意下原本是怎么表现的）
