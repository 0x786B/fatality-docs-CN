## cgame_ui_funcs

用法：`game.game_ui_funcs:{method}`

此类型代表游戏的UI函数。

## get_binding_for_button_code

[![Method][此字段是一个方法，必须使用冒号(:)来调用。]rw]

返回按钮代码对应的绑定名称。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `code` | `int` | 按钮代码。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `string` | 绑定。 |

**示例**

```lua
local bind = game.game_ui_funcs:get_binding_for_button_code(code);
```