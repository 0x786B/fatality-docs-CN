## 适配器

此类型表示渲染系统中使用的渲染适配器。

## 获取后缓冲区

返回后缓冲区纹理。如果后缓冲区纹理未更新，可能返回空白或过时的纹理。

**参数**

无。

**返回**

| 类型 | 描述 |
| ---- | ----------- |
| [`ptr`](/api/common-types/ptr "此类型是一个字面指针。") | 后缓冲区纹理指针。 |

**示例**

```lua
local bb = adapter:get_back_buffer();
```

## 获取降采样后缓冲区

返回后缓冲区纹理的4倍降采样版本。

**参数**

无。

**返回**

| 类型 | 描述 |
| ---- | ----------- |
| [`ptr`](/api/common-types/ptr "此类型是一个字面指针。") | 降采样后缓冲区纹理指针。 |

**示例**

```lua
local ds = adapter:get_back_buffer_downsampled();
```

## 获取共享纹理

返回共享纹理。此纹理通常复制降采样后的后缓冲区纹理，尽管它在图层渲染开始前自动更新一次。

**参数**

无。

**返回**

| 类型 | 描述 |
| ---- | ----------- |
| [`ptr`](/api/common-types/ptr "此类型是一个字面指针。") | 共享纹理指针。 |

**示例**

```lua
local shared = adapter:get_shared_texture();
```