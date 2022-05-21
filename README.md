# lua unicode utf16 to utf8
Forked from [Ko-Ta2142/lua_utf16: convert unicode(16le/be) ro utf8](https://github.com/Ko-Ta2142/lua_utf16).
Just package, and change interface here.
Test on Lua 5.3

------
original:

> unicode(16le/be)からutf8へ変換します。  
> bomがあれば自動判別します。
>
> convert unicode to utf8.
> bom auto detect.

## sample

```lua
local utf16_to_utf8=require'utf16_to_utf8'

-- exists bom
local utf8_string = utf16_to_utf8(utf16_string)

-- no bom
local utf8_string = utf16_to_utf8(utf16_string,true) --little edinet
```