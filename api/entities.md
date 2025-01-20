## entities

此表代表内部实体列表。

> 切勿在全局作用域中存储任何实体！任何实体都可能被删除，您将不再拥有该实体的有效实例，这将不可避免地导致崩溃。如果您需要在全局范围内存储实体，我们强烈建议您存储 [`chandle`](/api/entities/chandle "此类型表示实体句柄") 的实例，并在需要时使用其 [`get`](/api/entities/chandle?id=get "返回实体，如果未找到则返回 nil。") 方法重新获取实体。

## players

[![字段][这是一个必须使用点(.)访问的常规字段。]rw]

类型：[`entity_list_t<cs2_player_pawn>`](/api/entities/entity-list-t "此类型表示实体列表。")

玩家模型。

## controllers

[![字段][这是一个必须使用点(.)访问的常规字段。]rw]

类型：[`entity_list_t<cs2_player_controller>`](/api/entities/entity-list-t "此类型表示实体列表。")

玩家控制器。

## items

[![字段][这是一个必须使用点(.)访问的常规字段。]rw]

类型：[`entity_list_t<cs2_weapon_base>`](/api/entities/entity-list-t "此类型表示实体列表。")

物品（持有）。

## dropped_items

[![字段][这是一个必须使用点(.)访问的常规字段。]rw]

类型：[`entity_list_t<cs2_weapon_base>`](/api/entities/entity-list-t "此类型表示实体列表。")

掉落的物品。

## projectiles

[![字段][这是一个必须使用点(.)访问的常规字段。]rw]

类型：[`entity_list_t<cs2_grenade_projectile>`](/api/entities/entity-list-t "此类型表示实体列表。")

手榴弹投射物。

## get_local_pawn

[![函数][这是一个必须使用点(.)调用的常规函数。]rw]

返回本地玩家的模型。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| [`cs2_player_pawn`](/api/entities/base-entity/cs2-player-pawn "此类型表示 C_CSPlayerPawn 类。") | 玩家模型。 |

**示例**

```lua
local lp = entities.get_local_pawn();
```

## get_local_controller

[![函数][这是一个必须使用点(.)调用的常规函数。]rw]

返回本地玩家的控制器。

**参数**

无。

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| [`cs2_player_controller`](/api/entities/base-entity/cs2-player-controller "此类型表示 CCSPlayerController 类") | 控制器。 |

**示例**

```lua
local lp_ctrl = entities.get_local_controller();
```