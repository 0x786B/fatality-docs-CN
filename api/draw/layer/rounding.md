## rounding

此枚举用于确定圆角形状的圆角。

## tl

[![Field][此字段是一个普通字段，必须使用点(.)来访问。]rw]

圆角左上角。

## tr

[![Field][此字段是一个普通字段，必须使用点(.)来访问。]rw]

圆角右上角。

## bl

[![Field][此字段是一个普通字段，必须使用点(.)来访问。]rw]

圆角左下角。

## br

[![Field][此字段是一个普通字段，必须使用点(.)来访问。]rw]

圆角右下角。

## t

[![Field][此字段是一个普通字段，必须使用点(.)来访问。]rw]

圆角两个顶部角。这会产生与使用 `bit.bor(draw.rounding.tl, draw.rounding.tr)` 相同的结果。

## l

[![Field][此字段是一个普通字段，必须使用点(.)来访问。]rw]

圆角两个左侧角。这会产生与使用 `bit.bor(draw.rounding.tl, draw.rounding.bl)` 相同的结果。

## r

[![Field][此字段是一个普通字段，必须使用点(.)来访问。]rw]

圆角两个右侧角。这会产生与使用 `bit.bor(draw.rounding.tr, draw.rounding.br)` 相同的结果。

## b

[![Field][此字段是一个普通字段，必须使用点(.)来访问。]rw]

圆角两个底部角。这会产生与使用 `bit.bor(draw.rounding.bl, draw.rounding.br)` 相同的结果。

## all

[![Field][此字段是一个普通字段，必须使用点(.)来访问。]rw]

圆角所有角。这会产生与使用 `bit.bor(draw.rounding.tl, draw.rounding.tr, draw.rounding.bl, draw.rounding.br)` 相同的结果。