---
description: EventPlayerMove
---

# PlayerMove

Triggering an event when the player moves

Callback: `render_3d`

``

**Fields**

| Type      | Name |
| --------- | ---- |
| MoverType | type |
| double    | x    |
| double    | y    |
| double    | z    |



**Example**

****

```lua
--example
this:registerCallback("events" function(event)
	if event:getName() == "player_move" then
		mc.player:sendChatMessage("Veclocity X: " .. event.x)
		mc.player:sendChatMessage("Veclocity Y: " .. event.y)
		mc.player:sendChatMessage("Veclocity Z: " .. event.z)
	end
end)
```

