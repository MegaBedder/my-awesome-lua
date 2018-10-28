# My Awesome Lua List [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of quality Lua [packages](#packages) and [resources](#resources).

Inspired by the list [awesome-lua](https://github.com/LewisJEllis/awesome-lua).


## Packages
- [Implementations, Interpreters, and Bindings](#implementations-interpreters-and-bindings)
- [Package Managers](#package-managers)


## Resources
- [Complementary lists](#complementary-lists)


### Implementations, Interpreters, and Bindings
- [Lua](http://www.lua.org/download.html) - Lua's original ANSI C interpreter.
  - [Lua Repo](https://github.com/lua/lua) - The official Lua repo, as seen by the Lua team, mirrored to GitHub.
- [LuaJIT](http://luajit.org/luajit.html) - High-performance Just-In-Time compiler for Lua.


### Package Managers
- [LuaRocks](https://luarocks.org/) - De-facto tool for installing Lua modules as packages called "rocks", plus public rock repository and website.  Much like npm or pip.


### UNIX

### C ANSI standard
[lunary](https://luarocks.org/modules/doub/lunary) - A binary format I/O framework for Lua.

### C POSIX (Portable Operating System Interface) library
[luaposix](https://luarocks.org/modules/gvvaughan/luaposix) - Lua bindings for POSIX APIs.

[Lrexlib-POSIX](https://luarocks.org/modules/rrt/lrexlib-posix) - Lua binding of the POSIX regular expression library.

[nixio](https://luarocks.org/modules/luarocks/nixio) [[github]](https://github.com/jow-/lua-nixio) [[fork]](https://github.com/Neopallium/nixio)
 - is a multi-platform library for IPv4, IPv6 and UNIX networking, POSIX user/group management, TLS support.

[Berkeley Socket](https://en.wikipedia.org/wiki/Berkeley_sockets) (also known as BSD sockets) / [POSIX Sockets](http://pubs.opengroup.org/onlinepubs/9699919799/idx/networking.html) Interface

* <netinet/in.h>
  - Defines Internet protocol and address family (part of Berkeley sockets)

* <netinet/tcp.h>
  - Additional TCP control options (part of Berkeley sockets)

* <sys/socket.h>
  - Main Berkeley sockets header

```
Socket socket = getSocket(type = "TCP") -- creation of a socket
connect(socket, address = "1.2.3.4", port = "80") -- connecting to remote host
send(socket, "Hello, world!") -- sending the string
close(socket) -- and finally closing the socket
```

[X/Open Transport Interface](https://en.wikipedia.org/wiki/X/Open_Transport_Interface) (XTI)

> XTI provides similar functionality as the Berkeley sockets interface.
>
> - It is protocol independent in contrast to the socket interface which is heavily biased toward the [Internet Protocols](https://en.wikipedia.org/wiki/Internet_Protocol_Suite).
>
> - Is a transport service definition adhering to the [OSI model](https://en.wikipedia.org/wiki/OSI_model).
>
> XTI is now considered to be obsolete, so writers of new applications using the [Internet Protocol Suite (IPS)](https://en.wikipedia.org/wiki/Internet_Protocol_Suite) are recommended to use Sockets rather than XTI.
- [The Single UNIX® Specification (SUS), Version 2 (1997): Networking Services, Issue 5](http://pubs.opengroup.org/onlinepubs/7908799/xnsix.html)
- [Networking Services (XNS), Issue 5.2 Draft 2.0 (1999)](http://pubs.opengroup.org/onlinepubs/009619199/)

### Complementary lists
- [awesome-lua](https://github.com/LewisJEllis/awesome-lua) - A curated list of quality Lua packages and resources.
- [awesome-resty](https://github.com/bungle/awesome-resty) - A list like this one, but focused on OpenResty.
- [awesome-love2d](https://github.com/love2d-community/awesome-love2d) - A list like this one, but focused on game dev and the LÖVE platform.
- [Where Lua is Used](https://sites.google.com/site/marbux/home/where-lua-is-used) - A comprehensive list of stand-alone programs written in or extensible using Lua.
- [Where LuaJIT is Used](http://wiki.luajit.org/where-luajit-is-used) - Embeds, Supports, Implemented With LuaJIT


## Contribute

Contributions welcome and wanted! Read the [contribution guidelines](contributing.md) first.
