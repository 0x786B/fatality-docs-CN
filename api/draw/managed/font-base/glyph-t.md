## glyph_t

This type represents a glyph object.

## codepoint

[![Field][This field is a regular field that must be accessed using a dot (.).]rw]
[![Read Only][This field is a read only field, and you cannot change its value. This does not apply to child fields, if any.]r]

Type: `int`

Character codepoint.

## size

[![Field][This field is a regular field that must be accessed using a dot (.).]rw]
[![Read Only][This field is a read only field, and you cannot change its value. This does not apply to child fields, if any.]r]

Type: [`vec2`](https://lua.fatality.win/vec2.html "This type is a 2D vector used within the rendering system.")

Glyph dimensions.

## offset

[![Field][This field is a regular field that must be accessed using a dot (.).]rw]
[![Read Only][This field is a read only field, and you cannot change its value. This does not apply to child fields, if any.]r]

Type: [`vec2`](https://lua.fatality.win/vec2.html "This type is a 2D vector used within the rendering system.")

Glyph offset.

## uv

[![Field][This field is a regular field that must be accessed using a dot (.).]rw]
[![Read Only][This field is a read only field, and you cannot change its value. This does not apply to child fields, if any.]r]

Type: [`rect`](https://lua.fatality.win/rect.html "This type is a rectangle used within rendering system.")

UV rect on the texture atlas.