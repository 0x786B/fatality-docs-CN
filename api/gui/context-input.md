## context_input

此类型表示GUI输入上下文。

> 你可以在 [`input`](/api/events?id=input "每当GUI处理输入时都会调用。") 上下文之外使用 `cursor`、`is_mouse_up`、`is_mouse_down`、`is_key_up` 和 `is_key_down` 方法。使用其他方法没有意义，因为信息将是过时的。

## cursor

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

返回当前光标位置。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| [`vec2`](/api/draw/common-types/vec2 "这是渲染系统中使用的2D向量。") | 光标位置。 |

**示例**

```lua
local cur = gui.input:cursor();
```

## cursor_prev

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

返回上一个光标位置。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| [`vec2`](/api/draw/common-types/vec2 "这是渲染系统中使用的2D向量。") | 上一个光标位置。 |

**示例**

```lua
local prev = gui.input:cursor_prev();
```

## cursor_delta

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

返回上一个和当前光标位置之间的差值。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| [`vec2`](/api/draw/common-types/vec2 "这是渲染系统中使用的2D向量。") | 光标差值。 |

**示例**

```lua
local delta = gui.input:cursor_delta();
```

## did_cursor_move

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果光标自上次输入以来发生移动，则返回 `true`。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果移动则返回 `true`。 |

**示例**

```lua
if gui.input:did_cursor_move() then
    -- ...
end
```

## did_wheel_move

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果鼠标滚轮自上次输入以来发生移动，则返回 `true`。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果移动则返回 `true`。 |

**示例**

```lua
if gui.input:did_wheel_move() then
    -- ...
end
```

## did_process_mouse

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果任何鼠标按键的状态发生改变，则返回 `true`。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果处理了则返回 `true`。 |

**示例**

```lua
if gui.input:did_process_mouse() then
    -- ...
end
```

## button_released

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果自上次输入以来有任何按键被释放，则返回 `true`。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果释放则返回 `true`。 |

**示例**

```lua
if gui.input:button_released() then
    -- ...
end
```

## wheel_delta

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

返回此次输入滚动的行数。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `float` | 滚动的行数。 |

**示例**

```lua
local scroll = gui.input:wheel_delta();
```

## is_mouse_up

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果鼠标按键处于抬起状态（未按下），则返回 `true`。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `mb` | [`mouse_button`](/api/gui/context-input/mouse-button "此枚举表示鼠标按钮。") | 鼠标按钮。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果未按下则返回 `true`。 |

**示例**

```lua
if gui.input:is_mouse_up(gui.mouse_button.left) then
    -- ...
end
```

## is_mouse_down

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果鼠标按键处于按下状态，则返回 `true`。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `mb` | [`mouse_button`](/api/gui/context-input/mouse-button "此枚举表示鼠标按钮。") | 鼠标按钮。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果按下则返回 `true`。 |

**示例**

```lua
if gui.input:is_mouse_down(gui.mouse_button.left) then
    -- ...
end
```

## is_mouse_clicked

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果鼠标按键被点击（从未按下状态切换到按下状态），则返回 `true`。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `mb` | [`mouse_button`](/api/gui/context-input/mouse-button "此枚举表示鼠标按钮。") | 鼠标按钮。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果点击则返回 `true`。 |

**示例**

```lua
if gui.input:is_mouse_clicked(gui.mouse_button.left) then
    -- ...
end
```

## is_mouse_released

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果鼠标按键被释放（从按下状态切换到未按下状态），则返回 `true`。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `mb` | [`mouse_button`](/api/gui/context-input/mouse-button "此枚举表示鼠标按钮。") | 鼠标按钮。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果释放则返回 `true`。 |

**示例**

```lua
if gui.input:is_mouse_released(gui.mouse_button.left) then
    -- ...
end
```

## did_process_key

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果任何按键的状态发生改变，则返回 `true`。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果状态改变则返回 `true`。 |

**示例**

```lua
if gui.input:did_process_key() then
    -- ...
end
```

## is_key_up

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果按键处于抬起状态（未按下），则返回 `true`。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `k` | `int` | 虚拟按键。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果未按下则返回 `true`。 |

**示例**

```lua
if gui.input:is_key_up(0x41) then -- 'A' 键
    -- ...
end
```

## is_key_down

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果按键处于按下状态，则返回 `true`。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `k` | `int` | 虚拟按键。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果按下则返回 `true`。 |

**示例**

```lua
if gui.input:is_key_down(0x41) then -- 'A' 键
    -- ...
end
```

## is_key_clicked

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果按键被点击（从未按下状态切换到按下状态），则返回 `true`。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `k` | `int` | 虚拟按键。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果点击则返回 `true`。 |

**示例**

```lua
if gui.input:is_key_clicked(0x41) then -- 'A' 键
    -- ...
end
```

## is_key_released

[![方法][这是一个必须使用冒号(:)调用的方法。]rw]

如果按键被释放（从按下状态切换到未按下状态），则返回 `true`。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `k` | `int` | 虚拟按键。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `bool` | 如果释放则返回 `true`。 |

**示例**

```lua
if gui.input:is_key_released(0x41) then -- 'A' 键
    -- ...
end
```