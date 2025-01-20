## entity_entry_t

表示一个实体条目。

## entity

[![Field][这是一个常规字段，必须使用点(.)来访问。]rw]

类型: `<type>`

实体实例。类型取决于你获取它的列表。

## had_dataupdate

[![Field][这是一个常规字段，必须使用点(.)来访问。]rw]

类型: `bool`

如果客户端至少收到过一次此实体的更新，则为 `true`。

## handle

[![Field][这是一个常规字段，必须使用点(.)来访问。]rw]

类型: `chandle<type>`

实体的句柄。如果你需要全局访问某个实体，你**可以**将其存储在其他地方。

## avatar

[![Field][这是一个常规字段，必须使用点(.)来访问。]rw]

类型: `texture`

> 此字段仅在使用 `cs2_player_controller` 类型的条目上可用。

玩家的头像。如果尚未初始化，则为 `nil`。