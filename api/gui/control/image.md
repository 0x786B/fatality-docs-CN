## image

此类型表示一个图像控件。

> 此类型继承自 [`control`](/api/gui/control "此类型表示一个抽象的GUI控件。") 类型。其所有基础方法和字段在此类型中也可用。

## __call

[![构造函数][这是此类型的构造函数定义。]rw]

构造图像控件。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `id` | [`control_id`](/api/gui/common-types/control-id "此类型表示一个控件ID。") | ID。 |
| `tex` | [`texture`](/api/draw/managed/texture "此类型表示一个纹理对象。") | 纹理。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `image` | 图像实例。 |

**示例**

```lua
local img = gui.image(gui.control_id('my_id'));
```