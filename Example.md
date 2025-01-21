### 获取玩家列表

这里展示了如何封装一个用于获取玩家列表的函数和使用方法。

```lua
function entities.get_players(enemy)
    local players = {}
    entities.players:for_each(function(entry)
        if entry.handle:valid() then
            local player = entry.handle:get()
            if enemy then
                if player:is_enemy() then
                    table.insert(players, player)
                end
            else
                table.insert(players, player)
            end
        end
    end)
    return players
end
```

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `enemy` | `boolean` | （可选）如果为 true，则只返回敌人。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| `table[cs2_player_pawn]` | 包含玩家实体的数组[`cs2_player_pawn`](/api/entities/base-entity/cs2-player-pawn "类型: cs2_player_pawn")|

**用法示例**

```lua
-- 获取所有玩家
local all_players = entities.get_players()

-- 只获取敌人
local enemies = entities.get_players(true)

-- 遍历玩家
for _, player in ipairs(all_players) do
    -- 对每个玩家进行操作
    print(player:get_name())
end
```

**说明**

这个函数使用 `entities.players` 遍历所有玩家实体，并提供以下功能：

1. 检查实体句柄是否有效
2. 获取实体对象
3. 可选地过滤只返回敌人
4. 返回一个包含所有符合条件的玩家的数组

这个函数在需要对多个玩家进行操作时特别有用，比如：
- 获取所有敌人的位置
- 检查队友的状态
- 遍历所有玩家进行特定操作 