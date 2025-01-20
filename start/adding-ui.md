## 添加用户界面

现在您已经了解了基础知识，让我们通过允许用户切换文本来扩展我们的脚本。我们可以通过在菜单中添加一个**控件**来实现这一点。

## 创建控件

让我们首先创建一个简单的复选框：

```lua
local cb = gui.checkbox(gui.control_id('my_checkbox'));
```

每个控件都有一个**唯一ID**，UI 框架使用这个 ID 来区分容器中的控件。确保您的控件 ID 不会与其他控件冲突非常重要，否则可能会导致状态损坏或更糟。

要创建 ID，调用 [`gui.control_id`](/api/gui/common-types/control-id#call "构造 ID 结构。") 并传入所需的 ID。

然后，通过调用 [`gui.checkbox`](/api/gui/control/checkbox?id=__call "构造复选框。") 并传入您创建的 ID 结构来创建复选框。

## 构建行

默认情况下，控件通常放置在**行**中 - 以特定方式堆叠元素的布局。我们提供了一个简单的辅助函数 - [`gui.make_control`](/api/gui?id=make_control "将控件包装到由标签和特定控件组成的布局中。如果您希望控件显示得漂亮，应将此新控件添加到分组框中。此外，您可以向返回的控件添加任何额外的控件 - 这些控件将堆叠在初始控件的左侧...")。

```lua
local row = gui.make_control('My checkbox', cb);
```

## 将行添加到分组

准备好控件和行后，让我们将它们添加到一个分组中。

> 要查看分组和控件 ID，您可以在 SCRIPTS 选项卡中启用**调试模式**。

在这个示例中，我们将使用 `lua>elements a` 分组。首先在全局上下文中找到该分组：

```lua
local group = gui.ctx:find('lua>elements a');
```

然后调用其 [`add`](/api/gui/container?id=add "将控件添加到容器中。") 方法以包含您的行：

```lua
group:add(row);
```

就是这样！

## 使用值

接下来，让我们修改之前的脚本，使文本仅在复选框被选中时显示。在渲染文本之前，将绘图代码包装在 `if` 语句中：

```lua
if cb:get_value():get() then
```

并在之后关闭它。

最终的脚本应该看起来像这样：

```lua
local cb = gui.checkbox(gui.control_id('my_checkbox'));
local row = gui.make_control('My checkbox', cb);
local group = gui.ctx:find('lua>elements a');
group:add(row);

local function on_present_queue()
    if cb:get_value():get() then
        local d = draw.surface;
        d.font = draw.fonts['gui_main'];
        d:add_text(draw.vec2(50, 50),
            'hello world',
            draw.color.white()
        );
    end
end

events.present_queue:add(on_present_queue);
```