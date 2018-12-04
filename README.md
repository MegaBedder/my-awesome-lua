# My Awesome Lua List [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/master/media/badge.svg)](https://github.com/sindresorhus/awesome)

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
- [Cryptographic](#cryptographic)
- [Programming Paradigms](#programming-paradigms)
- [Libraries](#libraries)
- [Utilities](#utilities)
- [Miscellaneous](#miscellaneous)
- [Network](#network)
- [Events & threads](#events--threads)
- [Native OS APIs](#native-os-apis)

## Resources
- [Blogs / Sites](#blogs--sites)
- [Articles and publications](#articles-and-publications)
- [Guides / Tutorials](#guides--tutorials)
- [Frequently Asked Questions (FAQ)](#frequently-asked-questions-faq)
- [Complementary lists](#complementary-lists)

-----------------

### Implementations, Interpreters, and Bindings
- [Lua](http://www.lua.org/download.html) - Lua's original ANSI C interpreter.
  - [Lua Repo](https://github.com/lua/lua) - The official Lua repo, as seen by the Lua team, mirrored to GitHub.

### Dialects, flavors and implementations
- [Titan](http://titan-lang.org) - a programming language, designed to be a statically-typed, ahead-of-time compiled sister language to Lua.
  - [Pallene](https://github.com/pallene-lang/pallene) - a statically typed, ahead-of-time-compiled (AOT) sister language to Lua, with a focus on performance.
- [Terra](http://terralang.org/) - a low-level system programming language that is embedded in and meta-programmed by the Lua programming language.
- [Céu](http://www.ceu-lang.org/) - a reactive language that aims to offer a higher-level and safer alternative to C. “Structured Synchronous Reactive Programming”
- [Lua Implementations](http://lua-users.org/wiki/LuaImplementations) - Reimplementations of Lua compilers and interpreters.

### Lua 5
- [Agena](http://agena.sourceforge.net/) - based on Lua 5 C source, but has significant syntax differences
- [SquiLu](https://github.com/mingodad/squilu) - A mix between [Squirrel](http://squirrel-lang.org/) and Lua, trying to get the best of both. Squirrel scripting language modified with lua libraries
- [GSL Shell](https://www.nongnu.org/gsl-shell/) - an interactive command line interface that gives easy access to a collection of numeric algorithms and functions based on the GNU Scientific Library (GSL).

### Lua 5.1
- [LuaJIT](http://luajit.org/luajit.html) - High-performance Just-In-Time compiler for Lua.
  - [RaptorJIT](https://github.com/raptorjit/raptorjit) - A dynamic language for system programming (LuaJIT fork for Linux/x86-64 server applications)
- [Shine](https://github.com/richardhundt/shine) - a general purpose, dynamic, multi-paradigm programming language which is based on a [modified version](https://github.com/richardhundt/tvmjit) of the LuaJIT VM with features geared more to programming in the large.
- [Metalua](https://github.com/fab13n/metalua) - a compiler for a superset of the Lua 5.1 language, which supports compile-time metaprogramming.
- [Typed Lua](https://github.com/andremm/typedlua) (PhD Thesis) - An Optional Type System for Lua
  - [Typed Lua + OO Support](https://github.com/kevinclancy/typedlua) - A Class System for Typed Lua
  - [Typed Lua + IDE Support](https://gitlab.com/martanne/typedlua/tree/visitor)
- [Idle](http://idle.thomaslauer.com/) - At the core of Idle sits a tweaked and significantly enhanced version of Lua 5.1.
- [Firth](https://github.com/IonoclastBrigham/firth) [[BLOG]](http://web.archive.org/web/20160305085519/http://blog.ionoclast.com/2015/05/firth-pre-alpha-1-a-forth-like-language-for-dsl-creation/) - A simple Forth-like language intended for DSL creation, implemented in Lua.

### Lua 5.2
- [Killa](https://github.com/ex/Killa): a scripting language based in Lua 5.2 with a JavaScript-like syntax

### Lua 5.3
- [golua](https://github.com/Azure/golua) - A Lua 5.3 engine implemented in Go
- [Ravi](https://github.com/dibyendumajumdar/ravi) - a derivative of Lua 5.3 with limited optional static typing and features LLVM and Eclipse OMR powered JIT compilers.
- [Jual](http://sajonoso.github.io/jual/) - an embeddable Virtual Machine (VM) that implements the JualScript language (a subset of ECMA Script or JavaScript). The implementation is derived from Lua 5.3.

### Compiles to Lua
- [MoonScript](https://moonscript.org/) - A programmer friendly language that compiles to Lua.
- [Fennel](https://fennel-lang.org/) - a programming language that brings together the speed, simplicity, and reach of Lua with the flexibility of a lisp syntax and macro system.
- [Urn](https://urn-lang.com/) - a Lisp dialect with a focus on minimalism which compiles to Lua.

### Compiles to JS, asm.js or WebAssembly for Browser
  - [Brozula](https://github.com/creationix/brozula) - a LuaJIT bytecode interpreter that generates ES5 JavaScript.
  - [lua.vm.js](https://github.com/daurnimator/lua.vm.js) - Compile Lua via emscripten to asm.js. Originally by kripken (author of emscripten).
  - [Moonshine](http://moonshinejs.org/) - A lightweight Lua VM for the browser
  - [Starlight](http://starlight.paulcuth.me.uk/) - A Lua to ECMAScript 6 transpiler.
  - [lua5.1.js](https://github.com/logiceditor-com/lua5.1.js) - Lua 5.1, built with emscripten, with low-level API
  - [glua](https://github.com/fiatjaf/glua) - a Lua VM written in Go, to Javascript.
  - [ljs](http://code.matthewwild.co.uk/ljs) [[fork]](https://github.com/humbletim/ljs) - Lua VM implemented in Javascript
  - [lua.js](https://github.com/mherkender/lua.js) - Translate Lua code into Javascript.
  - [Fengari](https://fengari.io/) - Lua VM for the browser. This approach is the only viable one to use Lua in the browser and interact with the DOM.
  - [js2lua](https://github.com/wizzard0/js2lua) - Javascript to Lua translator, using LuaJIT
  - [LuaJS](https://github.com/Doridian/LuaJS) - Lua VM running in Javascript (using emscripten)
  - [Lua.js](https://github.com/tdzl2003/lua.js) - a project that can convert lua code to javascript. lua.js is fully written by javascript
  - [Luwa](https://github.com/serprex/luwa) - Lua WASM JIT
  - [wasm_lua](https://github.com/vvanders/wasm_lua) - Lua VM running in a WASM environment

### Distribution
- [Lua Binaries](http://luabinaries.sourceforge.net/) - a distribution of the Lua libraries and executables compiled for several platforms.
- [LuaWiMix](https://github.com/tDwtp/LuaWiMix) - A Lua distribution similar to LuaForWindows without anything but ilua, but with support for Lua 5.1 5.2 and 5.3 including optional luarocks and a switching mechanism.

### Package Managers
- [LuaRocks](https://luarocks.org/) - De-facto tool for installing Lua modules as packages called "rocks", public rock repository and website.
- [LuaDist](http://luadist.org/) -  a multi-platform package management system that aims to provide both source and binary repository of modules for Lua.
- [LuaPlus](http://luaplus.org) - Full LuaPlus distribution (fork of Lua 5.1) for Windows
- [ULua](http://ulua.io/) - Universal Lua Distribution
- [LuaPower](https://luapower.com/) - the LuaJIT distribution for Windows, Linux and OS X
- [Lit](https://github.com/luvit/lit/) [[web]](http://luvit.io/lit.html) - Toolkit for the ``Luvit`` ecosystem

### Batteries Included
- [Lua for Windows](https://github.com/rjpcomputing/luaforwindows) - a 'batteries included environment' for the Lua scripting language on Windows.
- [UFO - Un Finished Object](https://github.com/malkia/ufo) - a portable distribution of LuaJIT with precompiled binaries, libraries and FFI bindings
- [NekoLua](https://github.com/quinsmpang/NekoLua) - A distribution of Lua customized
- [Omnia](https://github.com/tongson/omnia) - Compile Lua, Fennel and MoonScript source code into standalone executables. Using ``luastatic``.

### Build Tools and Standalone Makers
- [srlua](https://github.com/LuaDist/srlua) - A tool for building self-running Lua programs.
- [luastatic](https://github.com/ers35/luastatic) - Build a standalone executable from a Lua program.
- [Luabuild](https://github.com/stevedonovan/luabuild) - A Custom Lua 5.2 Builder (tool to build a static Lua with bundled libraries)
- [slua](https://github.com/philanc/slua) - A static build of Lua 5.3 for Linux, with a few extension libraries.

-----------------

### I/O
- [lua-nixio](https://github.com/jow-/lua-nixio) [[fork]](https://github.com/Neopallium/nixio) - a multi-platform library for IPv4, IPv6 and UNIX networking, POSIX user/group management, TLS support. System, Networking and I/O library for Lua.
- [LuaSys](https://github.com/tnodir/luasys) - a portable Lua library providing access to system and networking functions.
- [Luvit](https://luvit.io/) - Lua + libUV + jIT = pure awesomesauce
- [Luver](https://github.com/squeek502/luver) - a ``luvit`` without ``lit``.
- [LuaNode](https://github.com/ignacio/LuaNode) - Asynchronous I/O for Lua
- [lunary](https://luarocks.org/modules/doub/lunary) - A binary format I/O framework for Lua.
- [binarystream](https://luarocks.org/modules/Tarik02/binarystream) - Lua library to work with binary data (needs ffi support)

### Data structures
- [Tuple](https://luarocks.org/modules/maia/tuple) - Tuple of Values for Lua.
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

### Cryptographic
- [lua-argon2](https://github.com/thibaultCha/lua-argon2) - the Argon2 password hashing function. Compatible with Lua 5.x and LuaJIT.
- [PLC](https://github.com/philanc/plc) (Pure Lua Crypto) - A small collection of crpytographic functions, and related utilities, implemented in pure Lua (version 5.3 or above)
- [Luazen](https://github.com/philanc/luazen) - a small library with various encoding, compression and cryptographic functions. All the functions work on strings, there is no stream or chunked more complex interfaces.
- [luatweetnacl](https://github.com/philanc/luatweetnacl) - Lua binding to the NaCl ("Tweet" version) crypto library

### File System
- [luafilesystem](https://github.com/keplerproject/luafilesystem) - LuaFileSystem complements the set of file system functions offered by the standard Lua distribution.

### Programming Paradigms
- Object-oriented programming
  - [30log](https://github.com/Yonaba/30log) - a small class system for OOP in Lua
  - [middleclass](https://github.com/kikito/middleclass) - A simple OOP library for Lua. It has inheritance, metamethods (operators), class variables and weak mixin support.
  - [LOOP](https://luarocks.org/modules/maia/loop) - Class Models for Lua
- Event-driven programming
  - [Luvent](https://github.com/ejmr/Luvent) - Simple Event Library for Lua
  - [lua_async](https://github.com/imwithye/lua_async) - Asynchronous and event driven programming in lua
  - [toynet](https://github.com/yongkangchen/toynet) - A simple event-driven I/O for Lua, coroutine based.
- Functional programming
  - [Lua Fun](https://github.com/luafun/luafun) - a high-performance functional programming library for Lua
  - [Moses](https://github.com/Yonaba/Moses) - Utility library for functional programming in Lua
- Reactive programming
  - [FRLua](https://luarocks.org/modules/aiverson/fr) - Functional Reactive programming capabilities in Lua.
  - [RxLua](https://luarocks.org/modules/bjornbytes/rxlua) - Reactive Extensions for Lua

### Libraries
- [lua-cjson](https://github.com/mpx/lua-cjson) - Lua CJSON is a fast JSON encoding/parsing module for Lua
- [LPegLabel](https://github.com/sqmedeiros/lpeglabel) - a conservative extension of the ``LPeg`` library that provides an implementation of Parsing Expression Grammars (PEGs) with labeled failures.
- [LPeg](http://www.inf.puc-rio.br/~roberto/lpeg/) - a new pattern-matching library for Lua, based on Parsing Expression Grammars (PEGs).
- [lualinq](https://luarocks.org/modules/djfdyuruiry/lualinq) - Lightweight library which allows functional querying and transformation of lua arrays and objects
- [base2base](https://github.com/catwell/base2base) - A pure Lua base-to-base converter
- [Libraries And Bindings](http://lua-users.org/wiki/LibrariesAndBindings) - a list of libraries implemented in Lua or implemented in another language (e.g. C) but having a Lua interface.

### Utilities
- [Allen](https://github.com/Yonaba/Allen) - An utility library to manipulate strings, which provides a set of helpers for strings operations for Lua.
- [Strictness](https://github.com/Yonaba/strictness) - a small module to track access and assignment to undefined variables in Lua

### Miscellaneous
- [Luno](https://luarocks.org/modules/echiesse/luno) - General purpose libraries for Lua.
- [lua-stdlib](https://github.com/lua-stdlib/lua-stdlib/) - General Lua libraries
- [Penlight](https://github.com/stevedonovan/Penlight) - A set of pure Lua libraries focusing on input data handling, functional programming, and OS path management. Inspired by the Python standard libraries.
- [Microlight](https://github.com/stevedonovan/microlight) - A little library of useful Lua functions, intended as the 'light' version of Penlight

### Network
- [lua-http](https://luarocks.org/modules/daurnimator/http) [[Video]](https://www.youtube.com/watch?v=OeABiyUlAao) - HTTP Library for Lua. Supports HTTP(S) 1.0, 1.1 and 2.0; client and server.
- [lua-websockets](https://github.com/lipp/lua-websockets) - This project provides Lua modules for Websocket Version 13 conformant clients and servers.
- [Ratchet](https://ratchet.icgood.net/) - The purpose of the ratchet library is to provide in Lua an asynchronous socket control mechanism for large numbers of sockets without using OS-level threads or losing the ease of synchronous socket programming.
- [Turbo](https://github.com/kernelsauce/turbo) - a framework built for LuaJIT 2 to simplify the task of building fast and scalable network applications. It uses a event-driven, non-blocking, no thread design to deliver excellent performance and minimal footprint to high-load applications.
- [LuaSocket](https://luarocks.org/modules/luarocks/luasocket) [[Doc]](https://htmlpreview.github.io/?https://raw.githubusercontent.com/diegonehab/luasocket/master/doc/index.html) - Network support for the Lua language
- [lsocket](https://luarocks.org/modules/gunnar_z/lsocket) - simple and easy socket support for lua.
- [llsocket](https://luarocks.org/modules/mah0x211/llsocket) - low-level socket module [this module is under heavy development]
- [lua-resty-socket](https://luarocks.org/modules/thibaultcha/lua-resty-socket) - A module offering interoperability between the LuaSocket and cosocket APIs
- [lua-net](https://luarocks.org/modules/rayaman/lua-net) - Lua networking library that wraps around lua-socket to make networking easy.
- [dromozoa-socks](https://luarocks.org/modules/moyu/dromozoa-socks) - Toolkit for network and I/O programming

### Events & threads
> for concurrent programming

- [lua-llthreads](https://github.com/Neopallium/lua-llthreads) - Low-Level threads (pthreads and WIN32 threads) for Lua.
- [lua-llthreads2](https://github.com/moteus/lua-llthreads2) - drop-in replacement for ``lua-llthreads`` library with several additional functionality.
- [luaproc](https://github.com/askyrme/luaproc) [[paper]](http://www.inf.puc-rio.br/~roberto/docs/ry08-05.pdf) - multi-threading library
- [Lua Lanes](https://github.com/LuaLanes/lanes) - a lightweight, native, lazy evaluating multithreading library for Lua 5.1 to 5.4.
- [Effil](https://github.com/effil/effil) [[slideshow]](http://www.lua.org/wshop18/Kupriyanov.pdf) - Multithreading support for Lua. It allows to spawn native threads and safe data exchange.
- [Copas](https://luarocks.org/modules/tieske/copas) - Dispatcher based on coroutines that can be used for asynchronous networking. (It uses LuaSocket for TCP/IP stack and LuaSec for SSL support)
- [cqueues](https://luarocks.org/modules/daurnimator/cqueues) - Continuation Queues: Embeddable asynchronous networking, threading, and notification framework for Lua on Unix.
- [lua-users: MultiTasking](http://lua-users.org/wiki/MultiTasking) - This page contains links and/or discussions related to multitasking/multithreading/parallelization in Lua.

### [Command Line](https://luarocks.org/labels/commandline) Specific
- [lcurses](https://github.com/lcurses/lcurses) - curses Terminal Screen Control
- [Readline](https://luarocks.org/modules/peterbillam/readline) - Interface to the readline library
- [linenoise](https://github.com/philanc/slua/tree/master/src/linenoise) - A small self-contained alternative to readline and libedit.
- [ljlinenoise](https://luarocks.org/modules/fperrad/ljlinenoise) - a pure LuaJIT port of [linenoise](https://github.com/antirez/linenoise), a small alternative to readline and libedit.

### Native OS APIs

### POSIX
- [luaposix](https://luarocks.org/modules/gvvaughan/luaposix) - Lua bindings for POSIX APIs.

### Windows-specific
- [winapi](https://github.com/stevedonovan/winapi) - Minimal Windows API
- [luapower/winapi](https://luapower.com/winapi) - Windows, common controls and dialogs, message loop and system APIs for LuaJIT.

### UNIX
- [ljsyscall](https://github.com/justincormack/ljsyscall) - Unix system calls for LuaJIT
- [minisock](https://github.com/philanc/minisock) - a minimal Lua socket library for unix / tcp / udp connections. The API is very close to the standard Unix system calls.
- [lunix](https://luarocks.org/modules/daurnimator/lunix) - Bindings to common Unix system APIs, striving for thread-safety.
- [luaunix](https://luarocks.org/modules/mbalmer/luaunix) - A Lua Binding for Selected Unix functions and System Calls
- [dromozoa-unix](https://luarocks.org/modules/moyu/dromozoa-unix) - Lua bindings for UNIX system interface

-----------------

### Blogs / Sites
- [Lua.Space](http://lua.space/) [[RSS Feed]](http://feeds.feedburner.com/Luaspace) - The Lua Community Blog
- [lua nova](https://luanova.org/) - welcome to the moon

### Articles and publications
- [A Look at the Design of Lua](https://cacm.acm.org/magazines/2018/11/232214-a-look-at-the-design-of-lua/fulltext) - 2018
- [Roberto Ierusalimschy • Publications](http://www.inf.puc-rio.br/~roberto/cvpub.html)
- [Programming with Multiple Paradigms in Lua](http://www.inf.puc-rio.br/~roberto/docs/ry09-03.pdf)
- [How uses Coroutines for non-blocking I/O](http://leafo.net/posts/itchio-and-coroutines.html) - It uses coroutines for all asynchronous operations like database queries and HTTP requests.
- [Interfacing Lua with C](https://ciel.im/posts/interfacing-lua-with-c/) - Lua provides an interface allowing to call C functions in Lua environment.
- [Asynchronous and Event-driven Programming in Lua](https://ciel.im/posts/asynchronous_lua/) - This article demonstrates how to bind libuv API to Lua environment.
- [Port Lua to Web Environment using WebAssembly (Wasm)](https://ciel.im/posts/port-lua-to-web-environment/) - using emscripten to compile Lua
- [Implementing Proper Getter/Setters in Lua](http://ebens.me/post/implementing-proper-gettersetters-in-lua) - a class in Lua (OOP)
- [Linked Lists in Lua](http://ebens.me/post/linked-lists-in-lua) - an example of creating custom data structures in Lua
- [Embeddable scripting with Lua](https://www.ibm.com/developerworks/linux/library/l-lua/index.html) - Lua offers high-level abstraction without losing touch with the hardware
- [Embed Lua for scriptable apps](https://www.ibm.com/developerworks/linux/library/l-embed-lua/index.html) - Incorporate application scripting using a small language built for the job

### Lua Workshop
- Lua Workshop 2016
  - [On the design of Lua](https://www.youtube.com/watch?v=QystqRlz6bw) - Roberto Ierusalimschy (PUC-Rio)
- [Roberto Ierusalimschy • Talks](http://www.inf.puc-rio.br/~roberto/talks/index.html)

### Guides / Tutorials
- [Programming in Lua (PiL)](http://www.lua.org/pil/) - The official book first edition was aimed at Lua 5.0 and remains largely relevant.
- [Lua-Users: Lua Tutorial](http://lua-users.org/wiki/LuaTutorial) - This tutorial is aimed at all newcomers to the language Lua. We start off with where to find relevant introductory material and then progress to using the language with tutorials in the [TutorialDirectory)](http://lua-users.org/wiki/TutorialDirectory).
- [TutorialsPoint.com: Lua Tutorial](https://www.tutorialspoint.com/lua/) - is designed for all those readers who are looking for a starting point to learn Lua. It has topics suitable for both beginners as well as advanced users.
- [RIP Tutorial: Lua](https://riptutorial.com/lua) - Getting started with Lua
- [The.Lua.Tutorial](http://luatut.com/) - An Introduction to Lua and The Crash Course to Lua.
- [LuaGuide](https://github.com/davisdude/LuaGuide/blob/master/LuaGuide.md) - A guide to help people learn Lua
- [Learn X in Y minutes: Where X=Lua](https://learnxinyminutes.com/docs/lua/) - Learn Lua in 15 Minutes
- [Lua for Programmers](http://ebens.me/2012/08/27/lua-for-programmers-part-1) - Language Essentials, Data and Standard Libraries, More Advanced Concepts and Tips and Tricks.
- [Phrogz: Learning Lua](http://phrogz.net/lua/index.html) - Learning Lua/From JS, Referenced Values, Metatables, and Simple Inheritance, and Pseudo-OOP Syntax and Scope.
- [Learn Lua the Hard Way](http://www.phailed.me/2011/02/learn-lua-the-hard-way-1/) - a person has never programmed before at all

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
