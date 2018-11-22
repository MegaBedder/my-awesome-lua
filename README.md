# My Awesome Lua List [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of quality Lua [packages](#packages) and [resources](#resources).

Inspired by the list [LewisJEllis/awesome-lua](https://github.com/LewisJEllis/awesome-lua) and [forhappy/awesome-lua](https://github.com/forhappy/awesome-lua).


## Packages
- [Implementations, Interpreters, and Bindings](#implementations-interpreters-and-bindings)
- [Package Managers](#package-managers)


## Resources
- [Complementary lists](#complementary-lists)


### Implementations, Interpreters, and Bindings
- [Lua](http://www.lua.org/download.html) - Lua's original ANSI C interpreter.
  - [Lua Repo](https://github.com/lua/lua) - The official Lua repo, as seen by the Lua team, mirrored to GitHub.
- [LuaJIT](http://luajit.org/luajit.html) - High-performance Just-In-Time compiler for Lua.
- [RaptorJIT](https://github.com/raptorjit/raptorjit) - A dynamic language for system programming (LuaJIT fork for Linux/x86-64 server applications)


### Package Managers
- [LuaRocks](https://luarocks.org/) - De-facto tool for installing Lua modules as packages called "rocks", plus public rock repository and website.  Much like npm or pip.

### Affecting Lua's Behaviour
- Data Structures
- Classes/Objects
- Error Handling
- Filter
- Function Handling
- Output Control
- Reflection
- Streams
- Sessions
- Variable handling

### Command Line Specific Extensions
- Ncurses — Ncurses Terminal Screen Control
- Newt (libnewt) - a programming library for color text mode, widget based user interfaces. 
- Readline — GNU Readline

### Compression and Archive
- Bzip2
- LZF
- Phar
- Rar — Rar Archiving
- Zip
- Zlib — Zlib Compression

### Cryptography Extensions
- CSPRNG
- Hash — HASH Message Digest Framework
- Mhash
- OpenSSL
- Password Hashing
- Sodium

### Database Extensions
- PDO
- SQLite3

### Date and Time Related Extensions
- Date/Time
- Calendar

### File System Related Extensions
- Fileinfo
- Directories

### Human Language and Character Encoding Support
### Image Processing and Generation
- Cairo
- Exif — Exchangeable image information
- GD (libgd) — Image Processing and GD
- Gmagick
- ImageMagick — Image Processing

### Mail Related Extensions
- SMTP
- IMAP
- POP3
- NNTP

### Mathematical Extensions
- BC Math (libbcmath) — BCMath Arbitrary Precision Mathematics
- GMP (gmplib) — GNU Multiple Precision

### Process Control Extensions and System program execution
- libeio
- libev
- libevent
- PCNTL — Process Control
- POSIX
- pthreads (and pthreads-win32)
- Shared Memory (shmop)

### Text Processing
- BBCode — Bulletin Board Code
- CommonMark
- Parle — Parsing and lexing
- PCRE — Regular Expressions (Perl-Compatible)
- POSIX Regex — Regular Expression (POSIX Extended)
- Strings

### Variable and Type Related Extensions
- Ctype — Character type checking

### Web Services
- OAuth
- REST
- SOAP
- XML-RPC

### Windows Only Extensions
- COM — COM and .Net (Windows)
- DCOM

### XML Manipulation
- DOM
- libXML

### GUI Extensions
- [libui](https://github.com/andlabs/libui)


### Network
- URLs
- JSON
- Sockets
- FTP

--
iconv
intl
Multibyte String (UTF-8)


### Utilities and Libraries
- [Allen](https://github.com/Yonaba/Allen) - An utility library to manipulate strings, which provides a set of helpers for strings operations for Lua.
- [Moses](https://github.com/Yonaba/Moses) - Utility library for functional programming in Lua
- [Strictness](https://github.com/Yonaba/strictness) - a small module to track access and assignment to undefined variables in Lua
- [30log](https://github.com/Yonaba/30log) - a small class system for OOP in Lua

### Debugging
- [MobDebug](https://github.com/pkulchenko/MobDebug) - Remote debugger for Lua.
- [Serpent](https://github.com/pkulchenko/serpent) - Lua serializer and pretty printer.

### Network
[LuaSocket](https://luarocks.org/modules/luarocks/luasocket) [[Doc]](https://rawgit.com/diegonehab/luasocket/master/doc/index.html) - Network support for the Lua language

[lsocket](https://luarocks.org/modules/gunnar_z/lsocket) - simple and easy socket support for lua.

[llsocket](https://luarocks.org/modules/mah0x211/llsocket) - low-level socket module [this module is under heavy development]

[lua-resty-socket](https://luarocks.org/modules/thibaultcha/lua-resty-socket) - A module offering interoperability between the LuaSocket and cosocket APIs

[lua-net](https://luarocks.org/modules/rayaman/lua-net) - Lua networking library that wraps around lua-socket to make networking easy.

[dromozoa-socks](https://luarocks.org/modules/moyu/dromozoa-socks) - Toolkit for network and I/O programming

### Events & threads
[lua-llthreads](https://github.com/Neopallium/lua-llthreads) - Low-Level threads (pthreads and WIN32 threads) for Lua.

[Copas](https://luarocks.org/modules/tieske/copas) - Dispatcher based on coroutines that can be used for asynchronous networking. (It uses LuaSocket for TCP/IP stack and LuaSec for SSL support)

[cqueues](https://luarocks.org/modules/daurnimator/cqueues) - Continuation Queues: Embeddable asynchronous networking, threading, and notification framework for Lua on Unix.

### UNIX
[lunix](https://luarocks.org/modules/daurnimator/lunix) - Bindings to common Unix system APIs, striving for thread-safety.

[luaunix](https://luarocks.org/modules/mbalmer/luaunix) - A Lua Binding for Selected Unix functions and System Calls

[dromozoa-unix](https://luarocks.org/modules/moyu/dromozoa-unix) - Lua bindings for UNIX system interface

### C ANSI standard
[lunary](https://luarocks.org/modules/doub/lunary) - A binary format I/O framework for Lua.

### C POSIX (Portable Operating System Interface) library
[luaposix](https://luarocks.org/modules/gvvaughan/luaposix) - Lua bindings for POSIX APIs.

[Lrexlib-POSIX](https://luarocks.org/modules/rrt/lrexlib-posix) - Lua binding of the POSIX regular expression library.

[nixio](https://luarocks.org/modules/luarocks/nixio) - System, Networking and I/O library for Lua.

> is a multi-platform library for IPv4, IPv6 and UNIX networking, POSIX user/group management, TLS support.

* [lua-nixio](https://github.com/jow-/lua-nixio)
* [nixio [fork]](https://github.com/Neopallium/nixio)

### Blogs / Sites
[Lua.Space](http://lua.space/) [[RSS Feed]](http://feeds.feedburner.com/Luaspace) - The Lua Community Blog

### Guides / Tutorials
- [LuaGuide](https://github.com/davisdude/LuaGuide/blob/master/LuaGuide.md) - A guide to help people learn Lua

### Complementary lists
- [awesome-lua](https://github.com/LewisJEllis/awesome-lua) - A curated list of quality Lua packages and resources.
- [awesome-resty](https://github.com/bungle/awesome-resty) - A list like this one, but focused on OpenResty.
- [nginx-resources](https://github.com/fcambus/nginx-resources) – Nginx web server (+ Lua), OpenResty and Tengine.
- [awesome-torch](https://github.com/carpedm20/awesome-torch) – Tutorials, projects and communities for [Torch](http://torch.ch/), a scientific computing framework for LuaJIT.
- [awesome-love2d](https://github.com/love2d-community/awesome-love2d) - A list like this one, but focused on game dev and the LÖVE platform.
- [Where Lua is Used](https://sites.google.com/site/marbux/home/where-lua-is-used) - A comprehensive list of stand-alone programs written in or extensible using Lua.
- [Where LuaJIT is Used](http://wiki.luajit.org/where-luajit-is-used) - Embeds, Supports, Implemented With LuaJIT


## Contribute

Contributions welcome and wanted! Read the [contribution guidelines](contributing.md) first.
