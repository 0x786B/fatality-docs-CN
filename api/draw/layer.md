| `maxs` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 药丸的右下角点。 |
| `radius_min` | `float` | 药丸圆角的最小半径。 |
| `radius_max` | `float` | 药丸圆角的最大半径。 |
| `cols` | `table[color, color]` | 渐变颜色，从下到上应用。 |
| `segments` | `int` | 近似圆角的分段数。默认为 `16`。 |

**返回**

无。

**示例**

```lua
layer:add_pill_multicolor(
    draw.vec2(50, 50), draw.vec2(150, 100),
    10, 20, {
        draw.color(255, 0, 0),
        draw.color(0, 0, 255)
    }, 16);
```

## add_shadow_line

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一个阴影线。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `r` | [`rect`](/api/draw/common-types/rect "此类型是渲染系统中使用的矩形。") | 阴影线的边界框。 |
| `dir` | [`shadow_dir`](/api/draw/layer/shadow-dir "此枚举用于确定 add_shadow_line 方法的阴影方向。") | 阴影方向。 |
| `a` | `float` | 最大不透明度。默认为 `0.25`。 |

**返回**

无。

**示例**

```lua
layer:add_shadow_line(
    draw.rect(50, 50, 150, 150), draw.shadow_dir.down, 0.25);
```

## add_shadow_rect

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一个带阴影的矩形。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `r` | [`rect`](/api/draw/common-types/rect "此类型是渲染系统中使用的矩形。") | 矩形。 |
| `radius` | `float` | 阴影距离，以像素为单位，向外。 |
| `bg` | `bool` | 是否为矩形绘制背景。默认为 `true`。 |
| `a` | `float` | 阴影的最大不透明度。默认为 `0.25`。 |

**返回**

无。

**示例**

```lua
layer:add_shadow_rect(
    draw.rect(50, 50, 150, 150), 15, true, 0.25);
```

## add_glow

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一个发光框。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `r` | [`rect`](/api/draw/common-types/rect "此类型是渲染系统中使用的矩形。") | 框矩形。 |
| `radius` | `float` | 发光距离，以像素为单位，向外。 |
| `c` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 发光颜色。 |
| `parts` | [`glow_parts`](/api/draw/layer/glow-parts "此枚举用于确定形状周围的发光部分应渲染哪些部分。") | 要启用的发光部分。默认为 `all`。 |

**返回**

无。

**示例**

```lua
layer:add_glow(draw.rect(50, 50, 150, 150), 15, draw.color(255, 0, 0));
```

## add_rect_filled_rounded

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一个填充的圆角矩形。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `r` | [`rect`](/api/draw/common-types/rect "此类型是渲染系统中使用的矩形。") | 矩形。 |
| `c` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 填充颜色。 |
| `amount` | `float` | 圆角量。 |
| `rnd` | [`rounding`](/api/draw/layer/rounding "此枚举用于确定圆角形状的圆角。") | 圆角模式。默认为 `all`。 |

**返回**

无。

**示例**

```lua
layer:add_rect_filled_rounded(
    draw.rect(50, 50, 150, 150),
    draw.color(255, 0, 0),
    10,
    draw.rounding.all
);
```

## add_rect_filled_rounded_multicolor

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一个填充的多色圆角矩形。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `r` | [`rect`](/api/draw/common-types/rect "此类型是渲染系统中使用的矩形。") | 矩形。 |
| `c` | `table[color, color, color, color]` | 填充颜色。按顺时针顺序使用，从左上角开始。 |
| `amount` | `float` | 圆角量。 |
| `rnd` | [`rounding`](/api/draw/layer/rounding "此枚举用于确定圆角形状的圆角。") | 圆角模式。默认为 `all`。 |

**返回**

无。

**示例**

```lua
layer:add_rect_filled_rounded_multicolor(
    draw.rect(50, 50, 150, 150), {
        draw.color(255, 0, 0),
        draw.color(0, 255, 0),
        draw.color(0, 0, 255),
        draw.color(255, 255, 0)
    },
    10,
    draw.rounding.all
);
```

## add_triangle

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一个描边三角形。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `a` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | A 点。 |
| `b` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | B 点。 |
| `c` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | C 点。 |
| `col` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 线条颜色。 |
| `thickness` | `float` | 线条厚度。默认为 `1.0`。 |
| `mode` | [`outline_mode`](/api/draw/layer/outline-mode "此枚举用于确定描边形状的描边模式。") | 描边模式。默认为 `inset`。 |

**返回**

无。

**示例**

```lua
layer:add_triangle(
    draw.vec2(50, 50),
    draw.vec2(25, 75),
    draw.vec2(75, 75),
    draw.color(255, 0, 0),
    1.0,
    draw.outline_mode.inset
);
```

## add_quad

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一个描边四边形。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `tl` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 左上角点。 |
| `tr` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 右上角点。 |
| `br` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 右下角点。 |
| `bl` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 左下角点。 |
| `c` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 线条颜色。 |
| `thickness` | `float` | 线条厚度。默认为 `1.0`。 |
| `mode` | [`outline_mode`](/api/draw/layer/outline-mode "此枚举用于确定描边形状的描边模式。") | 描边模式。默认为 `inset`。 |

**返回**

无。

**示例**

```lua
layer:add_quad(
    draw.vec2(50, 50),
    draw.vec2(150, 50),
    draw.vec2(150, 150),
    draw.vec2(50, 150),
    draw.color(255, 0, 0),
    1.0,
    draw.outline_mode.inset
);
```

## add_rect

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一个描边矩形。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `r` | [`rect`](/api/draw/common-types/rect "此类型是渲染系统中使用的矩形。") | 矩形。 |
| `c` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 线条颜色。 |
| `thickness` | `float` | 线条厚度。默认为 `1.0`。 |
| `mode` | [`outline_mode`](/api/draw/layer/outline-mode "此枚举用于确定描边形状的描边模式。") | 描边模式。默认为 `inset`。 |

**返回**

无。

**示例**

```lua
layer:add_rect(
    draw.rect(50, 50, 150, 150),
    draw.color(255, 0, 0),
    1.0,
    draw.outline_mode.inset
);
```

## add_circle

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一个描边圆形。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `center` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 中心点。 |
| `radius` | `float` | 圆形半径。 |
| `c` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 线条颜色。 |
| `segments` | `int` | 圆形分段。默认为 `36`。 |
| `fill` | `float` | 填充量。默认为 `1.0`。 |
| `thickness` | `float` | 线条厚度。默认为 `1.0`。 |
| `mode` | [`outline_mode`](/api/draw/layer/outline-mode "此枚举用于确定描边形状的描边模式。") | 描边模式。默认为 `inset`。 |

**返回**

无。

**示例**

```lua
layer:add_circle(
    draw.vec2(100, 100),
    50,
    draw.color(255, 0, 0),
    36,
    1.0,
    1.0,
    draw.outline_mode.inset
);
```

## add_line

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一条线。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `a` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 起点。 |
| `b` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 终点。 |
| `c` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 线条颜色。 |
| `thickness` | `float` | 线条厚度。默认为 `1.0` |

**返回**

无。

**示例**

```lua
layer:add_line(
    draw.vec2(50, 50),
    draw.vec2(150, 150),
    draw.color(255, 0, 0)
);
```

## add_line_multicolor

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一条多色线。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `a` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 起点。 |
| `b` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 终点。 |
| `c` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 起始颜色。 |
| `c2` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 结束颜色。 |
| `thickness` | `float` | 线条厚度。默认为 `1.0`。 |

**返回**

无。

**示例**

```lua
layer:add_line_multicolor(
    draw.vec2(50, 50),
    draw.vec2(150, 150),
    draw.color(255, 0, 0),
    draw.color(0, 0, 255),
    2.0
);
```

## add_rect_rounded

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加一个圆角填充矩形。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `r` | [`rect`](/api/draw/common-types/rect "此类型是渲染系统中使用的矩形。") | 矩形。 |
| `c` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 线条颜色。 |
| `amount` | `float` | 圆角量。 |
| `rnd` | [`rounding`](/api/draw/layer/rounding "此枚举用于确定圆角形状的圆角。") | 圆角模式。默认为 `all`。 |
| `thickness` | `float` | 线条厚度。默认为 `1.0`。 |
| `mode` | [`outline_mode`](/api/draw/layer/outline-mode "此枚举用于确定描边形状的描边模式。") | 描边模式。默认为 `inset`。 |

**返回**

无。

**示例**

```lua
layer:add_rect_rounded(draw.rect(50, 50, 150, 150),
    draw.color(255, 255, 255), 14);
```

## add_text

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

添加文本。

> 如果未设置字体，此函数将不执行任何操作。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `p` | [`vec2`](/api/draw/common-types/vec2 "此类型是渲染系统中使用的二维向量。") | 文本起始点。 |
| `text` | `string` | 文本。 |
| `c` | [`color`](/api/draw/common-types/color "此类型是渲染系统中使用的颜色。") | 文本颜色。 |
| `params` | [`text_params?`](/api/draw/layer/text-params "此类型用于确定文本对齐。") | 文本对齐参数。默认为 `nil`。 |

**返回**

无。

**示例**

```lua
layer:add_text(draw.vec2(50, 50), 'Hello world!', draw.color(255, 255, 255));
```

## override_clip_rect

[![方法][此字段是一个方法，必须使用冒号（:）调用。]rw]

覆盖剪辑矩形并支持交集。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `r` | [`rect?`](/api/draw/common-types/rect "此类型是渲染系统中使用的矩形。") | 新的剪辑矩形。 |
| `intersect` | `bool` | 此函数是否应将先前的矩形与新矩形相交。默认为 `true`。 |

**返回**

无。

**示例**

```lua
layer:override_clip_rect(draw.rect(50, 50, 150, 150));
```