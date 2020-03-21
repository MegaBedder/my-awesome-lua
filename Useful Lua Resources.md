There are many great free online resources for Lua including:

1. [lua.org](https://www.lua.org/)

2. A highly recommended detailed and authoritative introduction to all aspects of Lua programming by Lua's chief architect: [Programming in Lua, by Roberto Ierusalimschy](http://www.lua.org/pil/)
    
3. For an official definition of the Lua language, consult the [Lua 5.1 Reference Manual](http://www.lua.org/manual/5.1/), by R. Ierusalimschy, L. H. de Figueiredo, W. Celes.

4. [Lua Style Guide](https://github.com/Olivine-Labs/lua-style-guide)

5. [Learn Lua in 15 minutes](http://tylerneylon.com/a/learn-lua/)

6. Some options for linting
    * [lua-checker](https://code.google.com/p/lua-checker/)
    
    * [Lua Lint](http://lua-users.org/wiki/LuaLint)
    
    * [Lua Inspect](http://lua-users.org/wiki/LuaInspect)
    
    * [luacheck](https://github.com/mpeterv/luacheck)
    
    * [Detecting Undefined Variables](http://lua-users.org/wiki/DetectingUndefinedVariables)
    
    
# Ubuntu

> $ sudo apt-get update

First install Lua and Luarocks using Apt:

> $ sudo apt-get install lua5.3 liblua5.3-dev luarocks

Then install the Busted testing framework for Lua:

> $ luarocks install busted

If this fails, you may need to use sudo:

> $ sudo luarocks install busted
