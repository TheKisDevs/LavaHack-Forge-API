---
description: RenderGameOverlayEvent.Text
---

# Render2D

**Fields**

| Type      | Name          |
| --------- | ------------- |
| **float** | particalTicks |



**Example**

```lua
this:registerCallback("events", function(event) 
	if event:getName() == "render_2d" then
		renderer:text("CatLua 1.12.2", vec2d(1, 1), color(255, 255, 255, 255))
	end
end)
```



**How to get `particalTicks`**

```lua
event.particalTicks
```
