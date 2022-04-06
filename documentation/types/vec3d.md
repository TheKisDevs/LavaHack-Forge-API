# Vec3d

## Fields

| Type   | Name |
| ------ | ---- |
| double | x    |
| double | y    |
| double | z    |

## Methods

### vec3d(double x, double y, doube z): LuaVec2d

```lua
-- constructor
local vec = vec2d(54, 87, 5) -- x = 54, y = 87, z = 5
```

## Example

```lua
local vec = vec2d(54, 87, 5)
print("x: ", vec.x, ", y: ", vec.y, " z: ", vec.z) -- "x: 54, y: 87, z = 5"
vec.x = 100
print("x: ", vec.x, ", y: ", vec.y, " z: ", vec.z) -- "x: 100, y: 87, z: 5"
vec.z = vec.z + 1
print("x: ", vec.x, ", y: ", vec.y, " z: ", vec.z) -- "x: 100, y: 87, z: 6"
```
