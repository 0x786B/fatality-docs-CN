## 第一步

现在您已经了解了基本知识，是时候开始编写脚本了。

## 启动文本编辑器
随意使用您喜欢的文本编辑器：[Visual Studio Code](https://code.visualstudio.com/)、[Notepad++](https://notepad-plus-plus.org/downloads/)，甚至是简单的记事本。

本地脚本位于此处：`<CS2_目录>/game/csgo/fatality/scripts`。您可能会注意到还有一个 `lib` 目录，但我们稍后再讨论。

创建一个以 `.lua` 结尾的新文件，并开始您的脚本工作。

> `.ljbc` 格式不能从本地源加载。

## 编写您的第一个脚本

一个典型的"Hello world!"示例可能有点平淡，所以让我们尝试一些稍微高级一点的东西。

```lua
local function on_present_queue()
    local d = draw.surface;
    d.font = draw.fonts['gui_main'];
    d:add_text(draw.vec2(50, 50),
        'hello world',
         draw.color.white()
    );
end

events.present_queue:add(on_present_queue);
```

现在，让我们分解这个示例脚本：

### 定义回调函数

在这个示例中，我们定义了一个名为 `on_present_queue` 的函数。这是一个**回调函数**，它将在每个渲染帧被调用。

### 获取绘图表面

`draw.surface` 是一个全局绘图表面，允许您在屏幕上绘制各种图形和文本。

### 设置字体

`draw.fonts['gui_main']` 是一个预定义的字体，用于在用户界面中绘制文本。您可以稍后探索其他可用的字体。

### 添加文本

`d:add_text()` 方法用于在屏幕上绘制文本。它接受以下参数：
- 文本位置（使用 `draw.vec2` 创建的 2D 向量）
- 要显示的文本字符串
- 文本颜色（使用 `draw.color.white()` 创建的白色）

### 注册事件

`events.present_queue:add(on_present_queue)` 将我们的回调函数注册到渲染队列事件中。这意味着每次渲染帧时都会调用 `on_present_queue` 函数。

## 下一步

现在您已经编写了第一个脚本，请查看[添加用户界面](/start/adding-ui)部分，了解如何为您的脚本添加交互性控件。