# Globals

### getFps(): int

```lua
local currentFps = globals:getFps()
```

### getFrametime(): double

```lua
local frametime = globals:getFrametime() -- getFrametime equals 1.0 / getFps
```

### getPosition(): [Vec3d](types/vec2d.md)

```lua
local position = globals:getPosition()
```

### currentTime(): long

```lua
local currentTime = globals:currentTime()
```

### getServer(): String

Returns current server. If server is null then it returns _"none"._

```lua
local serverIp = globals:getServer()
```

### getUsername(): String

Returns player's username.

```lua
local username = globals:getUsername()
```

### getPing(): int

Returns player's ping

```lua
local ping = globals:getPing()
```

### getEntities(): List\<Entity>

Returns list of entities in the world

```lua
local entities = globals:getEntities()

-- in loop
for i = 0, entities:size() - 1 do
    print(entities:get(i):getName())
end
```

### getPlayerEntities(): List\<EntityPlayer>

Returns list of players in the world

```lua
local players = globals:getPlayerEntities()

-- in loop
for i = 0, players:size() - 1 do
    print(players:get(i):getName())
end
```

### getTileEntities(): List\<TileEntity>

Returns list of tile entities in the world

```lua
local players = globals:getTileEntities()
```

### instanceOf(Object obj, String clazz): boolean

Return is object an instance of the specified type.

```lua
print(globals:instanceOf(mc.player, "net.minecraft.entity.Entity")) -- true

print(globals:instanceOf(mc.player, "net.minecraft.block.Block")) -- false
```

### getBlock(double x, double y, double z): Block

Returns the block from coords

```lua
local block = globals:getBlock(45, 5, 546)
```

### getSphere(float range, boolean sphere, boolean hollow)

Returns a list of blocks from shpere for player&#x20;

```lua
local sphere = globals:getSphere(6, true, false)
```

### getScaledResolution(): ScaledResolution

```lua
local sr = globals:getScaledResolution()
print("Width: ", sr:getScaledWidth(), " | Height: ", sr:getScaledHeight())
```

### getModuleManager(): ModuleManager

```lua
local modules = globals:getModuleManager()
local module = modules:getModuleByName("AutoRer")
print(module:getName(), "'s state: ", module:isToggled())
```

### getKeyName(int keyCode): String

```lua
local keyName = globals:getKeyName(1)
```

### getCategories(): ArrayList\<Category>

```lua
local categories = globals:getCategories()
print(categories:contains(globals:getModuleManager():getModuleByName("AutoRer"))) -- true
```

### getMouseWheel(): int

```lua
local mouseWheel = globals:getMouseWheel()

if mouseWheel ~= 0 then
    print("mouseWheel ~= 0!")
end
```

### openGui(): void

```lua
local guiBuilder = GuiBuilder.new("gui?!")

globals:openGui(guiBuilder:build())
```
