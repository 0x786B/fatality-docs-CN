## events_t

用法：`mods.events.{method}`

此模块允许你管理自定义游戏内事件监听器。

> 请注意，游戏服务器**知道**你正在监听哪些事件。在内部，我们只监听那些无论如何都会以某种方式发送给客户端的事件。如果你决定监听服务器通常不期望的事件，在官方服务器上**可能**会导致问题。

## add_listener

[![Method][这是一个方法，必须使用冒号(:)来调用。]rw]

向监听器添加一个游戏事件。

> 在内部，我们监听以下事件：
> * `player_hurt`（玩家受伤）
> * `item_purchase`（物品购买）
> * `bullet_impact`（子弹碰撞）
> * `weapon_fire`（武器开火）
> * `bomb_beginplant`（开始安装炸弹）
> * `bomb_abortplant`（中止安装炸弹）
> * `bomb_planted`（炸弹已安装）
> * `bomb_defused`（炸弹已拆除）
> * `bomb_exploded`（炸弹爆炸）
> * `round_start`（回合开始）
> * `game_newmap`（新地图）
> * `map_shutdown`（地图关闭）
>
> 不需要将这些事件添加到监听器中。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `name` | `string` | 事件名称 |

**返回值**

无。

**示例**

```lua
mods.events:add_listener('round_end');
```