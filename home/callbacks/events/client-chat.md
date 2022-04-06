---
description: Same as forge ClientChatEvent event
---

# Client Chat

### `client_chat`

### Methods

| Type   | Name       |
| ------ | ---------- |
| String | getMessage |

### Example

```lua
local system = luajava:bindClass("java.lang.System")

this:registerCallback("events", function(event)
    if (event:getName() == "client_chat") then
        system.out:println("Your message is ", event:getMessage())
    end
end)
```
