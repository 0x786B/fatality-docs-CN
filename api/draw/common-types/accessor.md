## 访问器

此类型表示一种安全访问映射的方式。

> 请注意，`<type>` 表示此实例持有的特定类型。例如，`accessor<texture>` 表示 `get` 将返回一个 `texture` 实例，而 `set` 只接受 `texture` 类型作为其 `obj` 参数。

## __index

返回一个通过键访问的对象。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `key` | `string` | 对象键。 |

**返回**

| 类型 | 描述 |
| ---- | ----------- |
| `<type>` | 对象。 |

**示例**

```lua
local main_font = draw.fonts['gui_main'];

-- 这也可以
local main_font_2 = draw.fonts.gui_main;
```

## __newindex

通过键设置一个对象。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `key` | `string` | 对象键。 |
| `obj` | `<type>` | 对象。 |

**返回**

无。

**示例**

```lua
draw.fonts['my_font'] = my_font;

-- 这也可以
draw.fonts.my_font = my_font;
```