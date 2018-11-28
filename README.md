# My Awesome Lua List [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of quality Lua [packages](#packages) and [resources](#resources).

Inspired by the list [LewisJEllis/awesome-lua](https://github.com/LewisJEllis/awesome-lua) and [forhappy/awesome-lua](https://github.com/forhappy/awesome-lua).

## Main
- [Implementations, Interpreters, and Bindings](#implementations-interpreters-and-bindings)
- [Package Managers](#package-managers)
- [Build Tools and Standalone Makers](#build-tools-and-standalone-makers)

## Packages
- [I/O](#io)
- [Web Frameworks](#web-frameworks)
- [GUI](#gui)
- [Debugging](#debugging)
- [Utilities and Libraries](#utilities-and-libraries)
- [Network](#network)
- [Events & threads](#events--threads)
- [Native OS APIs](#native-os-apis)

## Resources
- [Articles and publications](#articles-and-publications)
- [Blogs / Sites](#blogs--sites)
- [Frequently Asked Questions (FAQ)](#frequently-asked-questions-faq)
- [Guides / Tutorials](#guides--tutorials)
- [Complementary lists](#complementary-lists)


### Implementations, Interpreters, and Bindings
### Major implementations
- [Lua](http://www.lua.org/download.html) - Lua's original ANSI C interpreter.
  - [Lua Repo](https://github.com/lua/lua) - The official Lua repo, as seen by the Lua team, mirrored to GitHub.
- [Typed Lua](https://github.com/andremm/typedlua) (PhD Thesis) - An Optional Type System for Lua
  - [Typed Lua + OO Support](https://github.com/kevinclancy/typedlua) - A Class System for Typed Lua
  - [Typed Lua + IDE Support](https://gitlab.com/martanne/typedlua/tree/visitor)
- [Titan](http://titan-lang.org) - a programming language, designed to be a statically-typed, ahead-of-time compiled sister language to Lua.
- [Pallene](https://github.com/pallene-lang/pallene) (a fork of the Titan) - a statically typed, ahead-of-time-compiled sister language to Lua, with a focus on performance.
- [Terra](http://terralang.org/) - a low-level system programming language that is embedded in and meta-programmed by the Lua programming language.
- [LuaJIT](http://luajit.org/luajit.html) - High-performance Just-In-Time compiler for Lua.
- [RaptorJIT](https://github.com/raptorjit/raptorjit) - A dynamic language for system programming (LuaJIT fork for Linux/x86-64 server applications)
- [golua](https://github.com/Azure/golua) - A Lua 5.3 engine implemented in Go
- [Shine](https://github.com/richardhundt/shine) - a general purpose, dynamic, multi-paradigm programming language which is based on, and extends, Lua (and LuaJIT VM) with features geared more to programming in the large.
- [Céu](http://www.ceu-lang.org/) - a reactive language that aims to offer a higher-level and safer alternative to C. “Structured Synchronous Reactive Programming”
- [Firth](https://github.com/IonoclastBrigham/firth) - A simple Forth-like language intended for DSL creation, implemented in Lua. [[1]](http://web.archive.org/web/20160305085519/http://blog.ionoclast.com/2015/05/firth-pre-alpha-1-a-forth-like-language-for-dsl-creation/)
- [Fennel](https://fennel-lang.org/) - a programming language that brings together the speed, simplicity, and reach of Lua with the flexibility of a lisp syntax and macro system.
- [Urn](https://urn-lang.com/) - a Lisp dialect with a focus on minimalism which compiles to Lua.
- [MoonScript](https://moonscript.org/) - A programmer friendly language that compiles to Lua.
- To Web (JS, asm.js, WASM)
  - [Brozula](https://github.com/creationix/brozula) - a LuaJIT bytecode compiler that generates ES5 JavaScript.
  - [lua.vm.js](https://github.com/daurnimator/lua.vm.js) - The Lua VM, on the Web (using the asm.js subset of JavaScript)
  - [Moonshine](http://moonshinejs.org/) - A lightweight Lua VM for the browser
  - [Starlight](http://starlight.paulcuth.me.uk/) - A Lua to ECMAScript 6 transpiler.
  - [lua5.1.js](https://github.com/logiceditor-com/lua5.1.js) - Lua 5.1, built with emscripten, with low-level API
  - [glua](https://github.com/fiatjaf/glua) - a Lua VM written in Go, to Javascript.
  - [ljs](http://code.matthewwild.co.uk/ljs) [[fork]](https://github.com/humbletim/ljs) - Lua VM implemented in Javascript
  - [lua.js](https://github.com/mherkender/lua.js) - Translate Lua code into Javascript.
  - [Fengari](https://fengari.io/) - Lua VM for the browser. This approach is the only viable one to use Lua in the browser and interact with the DOM.
  - [Lua.js](https://github.com/tdzl2003/lua.js) - a project that can convert lua code to javascript. lua.js is fully written by javascript
  - [Luwa](https://github.com/serprex/luwa) - Lua WASM JIT
  - [wasm_lua](https://github.com/vvanders/wasm_lua) - Lua VM running in a WASM environment
- [Lua Implementations](http://lua-users.org/wiki/LuaImplementations) - Reimplementations of Lua compilers and interpreters.

### Dialects / Lua Derivative
> Languages based on Lua. These languages are based on the Lua implementation (e.g. adapted VM).
- [Agena](http://agena.sourceforge.net/) - based on Lua 5 C source, but has significant syntax differences
- [SquiLu](https://github.com/mingodad/squilu) - A mix between [Squirrel](http://squirrel-lang.org/) and Lua, trying to get the best of both. Squirrel scripting language modified with lua libraries
- [Idle](http://idle.thomaslauer.com/) - At the core of Idle sits a tweaked and significantly enhanced version of Lua 5.1.
- [Metalua](https://github.com/fab13n/metalua) - a compiler for a superset of the Lua 5.1 language, which supports compile-time metaprogramming.
- [GSL Shell](https://www.nongnu.org/gsl-shell/) - an interactive command line interface that gives easy access to a collection of numeric algorithms and functions based on the GNU Scientific Library (GSL).
- [Killa](https://github.com/ex/Killa): a scripting language based in Lua 5.2 with a JavaScript-like syntax
- [Ravi](https://github.com/dibyendumajumdar/ravi) - a derivative of Lua 5.3 with limited optional static typing and features LLVM and Eclipse OMR powered JIT compilers.
- [Jual](http://sajonoso.github.io/jual/) - an embeddable Virtual Machine (VM) that implements the JualScript language (a subset of ECMA Script or JavaScript). The implementation is derived from Lua 5.3.

### Package Managers
- [LuaRocks](https://luarocks.org/) - De-facto tool for installing Lua modules as packages called "rocks", plus public rock repository and website.
- [Lit](https://github.com/luvit/lit/) [[web]](http://luvit.io/lit.html) - Package Manager for the Luvit ecosystem

### Build Tools and Standalone Makers
- [srlua](https://github.com/LuaDist/srlua) - A tool for building self-running Lua programs.
- [luastatic](https://github.com/ers35/luastatic) - Build a standalone executable from a Lua program.

### I/O
- [lua-nixio](https://github.com/jow-/lua-nixio) [[fork]](https://github.com/Neopallium/nixio) - System, Networking and I/O library for Lua.

> is a multi-platform library for IPv4, IPv6 and UNIX networking, POSIX user/group management, TLS support.

- [Luvit](https://luvit.io/) - Asynchronous I/O for Lua
- [LuaNode](https://github.com/ignacio/LuaNode) - Asynchronous I/O for Lua
- [lunary](https://luarocks.org/modules/doub/lunary) - A binary format I/O framework for Lua.

### Data structures
- [lua-users: Data Structures](http://lua-users.org/wiki/DataStructures) - Here are implementations of various data structures in Lua or related discussions.

### Web Frameworks
- [Lapis](http://leafo.net/lapis/) - A web framework for Lua or MoonScript, powered by OpenResty
- [Sailor](http://sailorproject.org/) - A Lua MVC web framework.
- [Ophal](https://ophal.org/) - The highly scalable Lua CMS/CMF and web platform
- [Orbit](http://keplerproject.github.io/orbit/) - an MVC web framework for Lua, based on WSAPI. [[1]](https://luanova.org/orbit1-2/)

### GUI
- [Yue](https://libyue.com/) - A library for creating native cross-platform GUI apps.
- [wxLua](http://wxlua.sourceforge.net/) - a wrapper around the [wxWidgets](http://www.wxwidgets.org/) cross-platform C++ GUI library.

### Debugging
- [MobDebug](https://github.com/pkulchenko/MobDebug) - Remote debugger for Lua.
- [Serpent](https://github.com/pkulchenko/serpent) - Lua serializer and pretty printer.
- [lua-marshal](https://github.com/richardhundt/lua-marshal) - fast table serialization for Lua

### Utilities and Libraries
- [Allen](https://github.com/Yonaba/Allen) - An utility library to manipulate strings, which provides a set of helpers for strings operations for Lua.
- [Moses](https://github.com/Yonaba/Moses) - Utility library for functional programming in Lua
- [Strictness](https://github.com/Yonaba/strictness) - a small module to track access and assignment to undefined variables in Lua
- [30log](https://github.com/Yonaba/30log) - a small class system for OOP in Lua
- [middleclass](https://github.com/kikito/middleclass) - A simple OOP library for Lua. It has inheritance, metamethods (operators), class variables and weak mixin support.
- [Lua Fun](https://github.com/luafun/luafun) - a high-performance functional programming library for Lua
- [lua-stdlib](https://github.com/lua-stdlib/lua-stdlib/) - General Lua libraries
- [Penlight](https://github.com/stevedonovan/Penlight) - A set of pure Lua libraries focusing on input data handling, functional programming, and OS path management. Inspired by the Python standard libraries.
- [Microlight](https://github.com/stevedonovan/microlight) - A little library of useful Lua functions, intended as the 'light' version of Penlight
- [Libraries And Bindings](http://lua-users.org/wiki/LibrariesAndBindings) - a list of libraries implemented in Lua or implemented in another language (e.g. C) but having a Lua interface.

### Network
- [LuaSocket](https://luarocks.org/modules/luarocks/luasocket) [[Doc]](https://rawgit.com/diegonehab/luasocket/master/doc/index.html) - Network support for the Lua language

- [lsocket](https://luarocks.org/modules/gunnar_z/lsocket) - simple and easy socket support for lua.

- [llsocket](https://luarocks.org/modules/mah0x211/llsocket) - low-level socket module [this module is under heavy development]

- [lua-resty-socket](https://luarocks.org/modules/thibaultcha/lua-resty-socket) - A module offering interoperability between the LuaSocket and cosocket APIs

- [lua-net](https://luarocks.org/modules/rayaman/lua-net) - Lua networking library that wraps around lua-socket to make networking easy.

- [dromozoa-socks](https://luarocks.org/modules/moyu/dromozoa-socks) - Toolkit for network and I/O programming

### Events & threads
- [lua-llthreads](https://github.com/Neopallium/lua-llthreads) - Low-Level threads (pthreads and WIN32 threads) for Lua.

- [Copas](https://luarocks.org/modules/tieske/copas) - Dispatcher based on coroutines that can be used for asynchronous networking. (It uses LuaSocket for TCP/IP stack and LuaSec for SSL support)

- [cqueues](https://luarocks.org/modules/daurnimator/cqueues) - Continuation Queues: Embeddable asynchronous networking, threading, and notification framework for Lua on Unix.

### Native OS APIs

### Windows-specific
- [winapi](https://luapower.com/winapi) - Windows, common controls and dialogs, message loop and system APIs.

### UNIX
- [lunix](https://luarocks.org/modules/daurnimator/lunix) - Bindings to common Unix system APIs, striving for thread-safety.

- [luaunix](https://luarocks.org/modules/mbalmer/luaunix) - A Lua Binding for Selected Unix functions and System Calls

- [dromozoa-unix](https://luarocks.org/modules/moyu/dromozoa-unix) - Lua bindings for UNIX system interface

### POSIX
- [luaposix](https://luarocks.org/modules/gvvaughan/luaposix) - Lua bindings for POSIX APIs.


### Blogs / Sites
- [Lua.Space](http://lua.space/) [[RSS Feed]](http://feeds.feedburner.com/Luaspace) - The Lua Community Blog
- [lua nova](https://luanova.org/) - welcome to the moon

### Articles and publications
- [A Look at the Design of Lua](https://cacm.acm.org/magazines/2018/11/232214-a-look-at-the-design-of-lua/fulltext)
- [How uses Coroutines for non-blocking I/O](http://leafo.net/posts/itchio-and-coroutines.html) - It uses coroutines for all asynchronous operations like database queries and HTTP requests.
- [A Look at the Design of Lua](https://cacm.acm.org/magazines/2018/11/232214-a-look-at-the-design-of-lua/fulltext)
- [Implementing Proper Getter/Setters in Lua](http://ebens.me/post/implementing-proper-gettersetters-in-lua) - a class in Lua (OOP)
- [Linked Lists in Lua](http://ebens.me/post/linked-lists-in-lua) - an example of creating custom data structures in Lua

### Guides / Tutorials
- [Programming in Lua (PiL)](http://www.lua.org/pil/) - The official book first edition was aimed at Lua 5.0 and remains largely relevant.
- [Lua-Users: Lua Tutorial](http://lua-users.org/wiki/LuaTutorial) - This tutorial is aimed at all newcomers to the language Lua. We start off with where to find relevant introductory material and then progress to using the language with tutorials in the [TutorialDirectory)](http://lua-users.org/wiki/TutorialDirectory).
- [TutorialsPoint.com: Lua Tutorial](https://www.tutorialspoint.com/lua/) - is designed for all those readers who are looking for a starting point to learn Lua. It has topics suitable for both beginners as well as advanced users.
- [The.Lua.Tutorial](http://luatut.com/) - An Introduction to Lua and The Crash Course to Lua.
- [LuaGuide](https://github.com/davisdude/LuaGuide/blob/master/LuaGuide.md) - A guide to help people learn Lua
- [Learn X in Y minutes: Where X=Lua](https://learnxinyminutes.com/docs/lua/) - Learn Lua in 15 Minutes
- [Lua for Programmers](http://ebens.me/2012/08/27/lua-for-programmers-part-1) - Language Essentials, Data and Standard Libraries, More Advanced Concepts and Tips and Tricks.
- [Phrogz: Learning Lua](http://phrogz.net/lua/index.html) - Learning Lua/From JS, Referenced Values, Metatables, and Simple Inheritance, and Pseudo-OOP Syntax and Scope.

### Frequently Asked Questions (FAQ)
- [Lua FAQ](http://www.lua.org/faq.html) - official Lua FAQ
- [Lua-Users FAQ](http://lua-users.org/wiki/LuaFaq) - unofficial Lua FAQ, it is maintained by the Lua community.
- [uFAQ](http://www.luafaq.org/) - Lua Unofficial FAQ

### Complementary lists
- [awesome-lua](https://github.com/LewisJEllis/awesome-lua) - A curated list of quality Lua packages and resources.
- [awesome-resty](https://github.com/bungle/awesome-resty) - A list like this one, but focused on OpenResty.
- [nginx-resources](https://github.com/fcambus/nginx-resources) – Nginx web server (+ Lua), OpenResty and Tengine.
- [awesome-torch](https://github.com/carpedm20/awesome-torch) – Tutorials, projects and communities for [Torch](http://torch.ch/), a scientific computing framework for LuaJIT.
- [awesome-love2d](https://github.com/love2d-community/awesome-love2d) - A list like this one, but focused on game dev and the LÖVE platform.
- [Where Lua is Used](https://sites.google.com/site/marbux/home/where-lua-is-used) - A comprehensive list of stand-alone programs written in or extensible using Lua.
- [Where LuaJIT is Used](http://wiki.luajit.org/where-luajit-is-used) - Embeds, Supports, Implemented With LuaJIT
- [Curlie: Lua](https://curlie.org/Computers/Programming/Languages/Lua/) - Collection of sites about Lua
- [Lua Tutorials and Courses](https://hackr.io/tutorials/learn-lua) - Top about Tutorials and Courses
- [Topics/Lua](https://github.com/topics/lua) - See more topics about Lua
- [Topics/LuaJIT](https://github.com/topics/luajit) - See more topics about LuaJIT

## Contribute

Contributions welcome and wanted! Read the [contribution guidelines](contributing.md) first.
