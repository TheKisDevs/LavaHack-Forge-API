# Vec2d

## Fields

| Type   | Name |
| ------ | ---- |
| double | x    |
| double | y    |

## Methods

### vec2d(double x, double y): LuaVec2d

```lua
-- constructor
local vec = vec2d(54, 87) -- x = 54, y = 87
```

## Example

```lua
local vec = vec2d(54, 87)
print("x: ", vec.x, ", y: ", vec.y) -- "x: 54, y: 87"
vec.x = 100
print("x: ", vec.x, ", y: ", vec.y) -- "x: 100, y: 87"
```
