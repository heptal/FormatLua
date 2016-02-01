## Summary

FormatLua formats lua code to a more readable form by using ~~[Lua Development Tools library](https://github.com/eclipse/koneki.ldt/tree/master/libraries)~~ [Paul Kulchenko's perl script](http://notebook.kulchenko.com/programming/lua-beautifier-in-55-lines-of-perl).

## Require
* ~~Lua~~ Perl

## Support System
* MacOSX
* Linux

## How to Use
* Select lua code and click menu Selection -> Format -> Format Lua Code
* Select lua code and press alt+l

### Configure Setting
Setting ~~lua~~ perl path in FormatLua.sublime-settings

```json
{
    "perl_path": "/usr/bin/perl"
}
```
### Configure Key Binding
Add the following line to keymap settings

```json
{ "keys": ["alt+l"], "command": "format_lua" }
```

## Example
Original:

```lua
local a = "你好"
    local b
    function set_text(name, value)
            local doc = document:getElementsByName(name)
        if doc and #doc > 0 then
        doc[1]:setPropertyByName("text", value)
    end
    end
    return b
```
Formated:

```lua
local a = "你好"
local b
function set_text(name, value)
    local doc = document:getElementsByName(name)
    if doc and #doc > 0 then
        doc[1]:setPropertyByName("text", value)
    end
end
return b
```
