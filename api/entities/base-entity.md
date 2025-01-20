## base_entity

此类型表示一个基础游戏实体。

> 此类型可能会被返回给任何其他抽象实体类，但在内部会指向正确的类型。

## __index

[![Function][此字段是一个函数，必须使用点(.)来调用]rw]

尝试在此类中搜索字段。

**参数**

| 名称 | 类型 | 描述 |
| ---- | ---- | ----------- |
| `name` | `string` | 字段名称。 |

**返回值**

| 类型 | 描述 |
| ---- | ----------- |
| [`schema_accessor_t`](/api/entities/base-entity/schema-accessor-t "此类型表示一个特殊的结构，它引用实体对象中的某个字段。") | 访问器实例。 |

**示例**

```lua
local health = player.m_iHealth;
local health = player['m_iHealth']; -- 这种方式也可以
```