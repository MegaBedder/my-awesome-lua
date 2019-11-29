# My Awesome Lua List [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/master/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of quality Lua [packages](#packages) and [resources](#resources).

Inspired by the list [LewisJEllis/awesome-lua](https://github.com/LewisJEllis/awesome-lua) and [forhappy/awesome-lua](https://github.com/forhappy/awesome-lua).

## Main
- [Implementations, Interpreters, and Bindings](#implementations-interpreters-and-bindings)
- [Distribution](#distribution)
- [Package Managers](#package-managers)
- [Build Tools and Standalone Makers](#build-tools-and-standalone-makers)
- [IDE, Plugins and text editor](#ide-plugins-and-text-editor)

## Packages
- [Data structures](#data-structures)
- [Programming Paradigms](#programming-paradigms)
- [I/O](#io)
- [CLI](#cli)
- [GUI](#gui)
- [Debugging](#debugging)
- [Testing](#testing)
- [Cryptographic](#cryptographic)
- [File System](#file-system)
- [Network](#network)
- [Message broker / queues](#message-broker--queues)
- [Database drivers](#database-drivers)
- [Multitasking](#multitasking)
- [Native OS APIs](#native-os-apis)
- [Libraries](#libraries)
- [Utilities](#utilities)
- [Miscellaneous](#miscellaneous)

## Projects
- [Asynchronous I/O](#asynchronous-io)
- [Web Browser](#web-browser)
- [Web Plataforms](#web-plataforms)
- [Web Frameworks](#web-frameworks)
- [Game Framework](#game-framework)
- [Scientific Computing](#scientific-computing)
- [Digital Signal processing](#digital-signal-processing)
- [Miscellaneous](#miscellaneous)

## Resources
- [Blogs / Sites](#blogs--sites)
- [Style Guides](#style-guides)
- [Guides / Tutorials](#guides--tutorials)
- [Lua Workshop](#lua-workshop)
- [Articles](#articles)
- [Publications and Researchs](#publications-and-researchs)
- [Lua Technical Notes](#lua-technical-notes)
- [Books](#books)
- [Lua VM and Bytecode](#lua-vm-and-bytecode)
- [Glossaries](#glossaries)
- [Frequently Asked Questions (FAQ)](#frequently-asked-questions-faq)
- [Complementary lists](#complementary-lists)

-----------------

### Implementations, Interpreters, and Bindings
- [Lua](http://www.lua.org/download.html) - Lua's original ANSI C interpreter.
  - [Lua Repo](https://github.com/lua/lua) - The official Lua repo, as seen by the Lua team, mirrored to GitHub.

### Dialects, flavors and implementations
- [Terra](http://terralang.org/) - a low-level system programming language that is embedded in and meta-programmed by the Lua programming language.
- [SquiLu](https://github.com/mingodad/squilu) - A mix between [Squirrel](http://squirrel-lang.org/) 3.0.4 and Lua 5.1.5, trying to get the best of both. Squirrel scripting language modified with lua libraries
- [Céu](http://www.ceu-lang.org/) - a reactive language that aims to offer a higher-level and safer alternative to C. “Structured Synchronous Reactive Programming”
- [Lua Implementations](http://lua-users.org/wiki/LuaImplementations) - Reimplementations of Lua compilers and interpreters.

### Lua 5.1
- [LuaJIT](http://luajit.org/luajit.html) - High-performance Just-In-Time compiler for Lua.
  - [LuaJIT 2](https://github.com/openresty/luajit2) - OpenResty's Branch of LuaJIT 2 (fork)
  - [RaptorJIT](https://github.com/raptorjit/raptorjit) - A dynamic language for system programming (LuaJIT fork for Linux/x86-64 server applications)
  - [Moonjit](https://github.com/moonjit/moonjit) - JIT Compiler for the Lua. Fork of LuaJIT to continue development
  - [LuaVela](https://github.com/iponweb/luavela) [[BLOG]](https://eliasdaler.github.io/luavela/) - an implementation of Lua 5.1 based on LuaJIT 2.0, for Linux x86-64 only.
  - [LjTools](https://github.com/rochus-keller/LjTools) - LuaJIT Assembler/Disassembler - Tool to study LuaJIT 2.0 Bytecode with GUI
- [Shine](https://github.com/richardhundt/shine) - a general purpose, dynamic, multi-paradigm programming language which is based on a [modified version](https://github.com/richardhundt/tvmjit) of the LuaJIT VM with features geared more to programming in the large.
- [Metalua](https://github.com/fab13n/metalua) - a compiler for a superset of the Lua 5.1 language, which supports compile-time metaprogramming.
- [Typed Lua](https://github.com/andremm/typedlua) (PhD Thesis) - An Optional Type System for Lua
  - [Typed Lua + OO Support](https://github.com/kevinclancy/typedlua) - A Class System for Typed Lua
  - [Typed Lua + IDE Support](https://gitlab.com/martanne/typedlua/tree/visitor)
- [Idle](http://idle.thomaslauer.com/) - At the core of Idle sits a tweaked and significantly enhanced version of Lua 5.1. Includes a GUI module, built from scratch; usable ("good enough") to create simple GUIs and dialog boxes. 
- [Agena](http://agena.sourceforge.net/) - based on Lua 5.1 C source, but has significant syntax differences
- [GSL Shell](https://www.nongnu.org/gsl-shell/) - an interactive command line interface that gives easy access to a collection of numeric algorithms and functions based on the GNU Scientific Library (GSL).
- [Firth](https://github.com/IonoclastBrigham/firth) [[BLOG]](http://web.archive.org/web/20160305085519/http://blog.ionoclast.com/2015/05/firth-pre-alpha-1-a-forth-like-language-for-dsl-creation/) - A simple Forth-like language intended for DSL creation, implemented in Lua.

### Lua 5.2
- [Killa](https://github.com/ex/Killa): a scripting language based in Lua 5.2 with a JavaScript-like syntax

### Lua 5.3
- [Titan](http://titan-lang.org) [[Slides]](http://www.lua.org/wshop17/Gualandi.pdf) - a system programming language, designed to be a statically-typed, ahead-of-time (AOT) compiled sister language to Lua, focused on performance. It is designed to seemlessly interoperate with Lua.
  - [Pallene](https://github.com/pallene-lang/pallene) [[Paper]](http://www.inf.puc-rio.br/~roberto/docs/pallene-sblp.pdf) [[Slides]](https://gligneul.github.io/luaworkshop2018/) - a statically typed, ahead-of-time (AOT) compiled sister language to Lua, with a focus on performance. Pallene is also designed to seamlessly interoperate with Lua.
- [Ravi](https://github.com/dibyendumajumdar/ravi) [[Slides]](http://www.lua.org/wshop15/Majumdar.pdf) [[Video]](https://www.youtube.com/watch?v=-ZOBHw1Mk2U) - a derivative of Lua 5.3 with limited optional static typing and features LLVM and Eclipse OMR powered JIT compilers.
- [golua](https://github.com/Azure/golua) - A Lua 5.3 engine implemented in Go by Azure
- [DCLua](https://github.com/milochristiansen/lua) - A Lua 5.3 VM and compiler written in Go.
- [Jual](http://sajonoso.github.io/jual/) - an embeddable Virtual Machine (VM) that implements the JualScript language (a subset of ECMA Script or JavaScript). The implementation is derived from Lua 5.3.

### Compiles to Lua
- [MoonScript](https://moonscript.org/) - A programmer friendly language that compiles to Lua 5.1.
- [Fennel](https://fennel-lang.org/) - a programming language that brings together the speed, simplicity, and reach of Lua with the flexibility of a lisp syntax and macro system.
- [Urn](https://urn-lang.com/) - a Lisp dialect with a focus on minimalism which compiles to Lua.

### Lua VM in Lua
- [LuLu](http://lulu.luaforge.net/) - a Lua 5.1 VM implementation in Lua language itself. Implements a VM interpreter and coroutine library, but reuses the host Lua environment for data types and standard library functions. 
- [Yueliang](http://yueliang.luaforge.net/) - Lua 5 in Lua 5 (5.0 and 5.1). The focus is on the front end of Lua, i.e. the lexical analyzer, the parser and the code generator, in order to generate binary chunks.
- [LuaVM](https://github.com/ds84182/LuaVM) - Lua Virtual Machine (and various tools) for Lua
- [LuaJIT Language Toolkit](https://github.com/franko/luajit-lang-toolkit) - an implementation of the Lua programming language written in Lua itself, as a starting point to implement a programming language that targets the LuaJIT virtual machine.

### Compiles to JS, asm.js or WebAssembly for Browser
  - [Brozula](https://github.com/creationix/brozula) - a LuaJIT bytecode interpreter that generates ES5 JavaScript.
  - [Fengari](https://fengari.io/) - Lua VM for the browser. A viable approach to using Lua in the browser and interacting with the DOM.
  - [glua](https://github.com/fiatjaf/glua) - a Lua VM written in Go, to Javascript.
  - [ljs](http://code.matthewwild.co.uk/ljs) [[fork]](https://github.com/humbletim/ljs) - Lua VM implemented in Javascript
  - [Lua.js](https://github.com/tdzl2003/lua.js) - a project that can convert lua code to javascript. lua.js is fully written by javascript
  - [lua.vm.js](https://github.com/daurnimator/lua.vm.js) - Compile Lua via emscripten to asm.js. Originally by kripken (author of emscripten).
  - [lua5.1.js](https://github.com/logiceditor-com/lua5.1.js) - Lua 5.1, built with emscripten, with low-level API
  - [LuaJS](https://github.com/Doridian/LuaJS) - Lua VM running in Javascript (using emscripten)
  - [Luwa](https://github.com/serprex/luwa) - Lua WASM JIT, a Lua runtime on top of WASM
  - [Moonshine](http://moonshinejs.org/) - A lightweight Lua VM for the browser
  - [wasm_lua](https://github.com/vvanders/wasm_lua) - Lua VM running in a WASM environment

### Transpiler Lua to JS and vice versa
  - [js2lua](https://github.com/wizzard0/js2lua) - Javascript to Lua translator, using LuaJIT
  - [lua.js](https://github.com/mherkender/lua.js) - Translate Lua code into Javascript.
  - [Starlight](http://starlight.paulcuth.me.uk/) - A Lua to ECMAScript 6 transpiler.

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
- [omnia](https://github.com/tongson/omnia) - A batteries-included creator of standalone executables, built on top of luastatic.
- [Lake](https://github.com/stevedonovan/Lake) - A build engine written in Lua, similar to Ruby's rake.
- [Luabuild](https://github.com/stevedonovan/luabuild) - A Custom Lua 5.2 Builder (tool to build a static Lua with bundled libraries)
- [slua](https://github.com/philanc/slua) - A static build of Lua 5.3 for Linux, with a few extension libraries.
- [Luapak](https://github.com/jirutka/luapak) - a command-line tool, multi-platform, adjustable, all-in-one (yet modular) solution for building a standalone, zero-dependencies, possibly statically linked (only on Linux) executable for (almost) any Lua program.

### IDE, Plugins and text editor
- [ZeroBrane Studio](https://studio.zerobrane.com/) - a lightweight Lua IDE with code completion, syntax highlighting, live coding, code analyzer, and debugging support for Lua 5.x, LuaJIT, and other Lua engines.
- [Lua Development Tools (LDT)](https://www.eclipse.org/ldt/) -  project provides plug-ins that implement a Lua IDE supporting the development of Lua scripts and applications. It adds a dedicated Lua perspective to the Eclipse Workbench, which, together with features such as syntax highlighting, scope-aware code completion, code folding, etc.
- [Lua for IDEA](https://bitbucket.org/sylvanaar2/lua-for-idea/wiki/Home) - IntelliJ IDEA plugin which, among other things, provides code completion, smart highlighting, and experimental debugging.
- [vscode-lua](https://github.com/trixnz/vscode-lua) - VSCode intellisense and linting.
- [Textadept](https://foicica.com/textadept/) - A fast, minimalist, and remarkably extensible cross-platform text editor
- [Howl Editor](https://howl.io/) - A general purpose, fast and lightweight editor with a keyboard-centric minimalistic user interface. Built on LuaJIT and fully programmable using Lua or Moonscript.
- [SciTE](https://www.scintilla.org/SciTE.html) - a SCIntilla based Text Editor, with embedded Lua interpreter.

-----------------

### Data structures
> Tables in Lua are not a data structure; they are the data structure.
- [Tuple](https://luarocks.org/modules/maia/tuple) - Tuple of Values for Lua.
- [array.lua](https://github.com/EvandroLG/array.lua) - A small library with useful methods to handle Lua's table when it's working like an Array
- [binarystream](https://luarocks.org/modules/Tarik02/binarystream) - Lua library to work with binary data (needs ffi support)
- [lua-users: Data Structures](http://lua-users.org/wiki/DataStructures) - Here are implementations of various data structures in Lua or related discussions.

### Programming Paradigms
- Object-oriented programming (OOP)
  - [30log](https://github.com/Yonaba/30log) - a small class system for OOP in Lua
  - [middleclass](https://github.com/kikito/middleclass) - A simple OOP library for Lua. It has inheritance, metamethods (operators), class variables and weak mixin support.
  - [LOOP](https://luarocks.org/modules/maia/loop) - Class Models for Lua
  - [PLoop](https://github.com/kurapica/PLoop) - a C# like style object-oriented program system for lua.
  - Aspect-oriented programming (AOP)
    - [RE-AspectLua](http://aspectlua.luaforge.net/) [[Paper]](http://www.scielo.br/scielo.php?script=sci_arttext&pid=S0104-65002006000100002) - a Lua 5.1 extension that allows the declaration of aspects.
- Event-driven programming
  - [Luvent](https://github.com/ejmr/Luvent) - Simple Event Library for Lua
  - [lua_async](https://github.com/imwithye/lua_async) - Asynchronous and event driven programming in lua
  - [toynet](https://github.com/yongkangchen/toynet) - A simple event-driven I/O for Lua, coroutine based.
  - [Reactor design pattern](https://en.wikipedia.org/wiki/Reactor_pattern)
    - [lua-reactor](https://luarocks.org/modules/talldan/reactor) - React-style ui component system for Lua
    - [lua-reactor-light](https://github.com/rimar/lua-reactor-light) - Lightweight lua reactor. Depends only on luasocket and exposes NodeJS-style API
- Functional programming
  - [Lua Fun](https://github.com/luafun/luafun) - a high-performance functional programming library for Lua
  - [Moses](https://github.com/Yonaba/Moses) - Utility library for functional programming in Lua
  - [lamda](https://github.com/helpermethod/lamda) - A functional programming library for Lua, inspired by Ramda.
- Reactive programming
  - [FRLua](https://luarocks.org/modules/aiverson/fr) - Functional Reactive programming capabilities in Lua.
  - [RxLua](https://luarocks.org/modules/bjornbytes/rxlua) - Reactive Extensions for Lua
- Defensive programming
  - [Safer](https://github.com/hishamhm/safer) - Paranoid Lua programming

-----------------

### I/O
- [lunary](https://luarocks.org/modules/doub/lunary) - A binary format I/O framework for Lua.
- [lua-nixio](https://github.com/jow-/lua-nixio) [[fork]](https://github.com/Neopallium/nixio) - a multi-platform library for IPv4, IPv6 and UNIX networking, POSIX user/group management, TLS support. System, Networking and I/O library for Lua.
- [LuaSys](https://github.com/tnodir/luasys) - a portable Lua library providing access to system and networking functions.

### [CLI](https://luarocks.org/labels/commandline)
- [lcurses](https://github.com/lcurses/lcurses) - curses Terminal Screen Control
- [Readline](https://luarocks.org/modules/peterbillam/readline) - Interface to the readline library
- [linenoise](https://github.com/philanc/slua/tree/master/src/linenoise) - A small self-contained alternative to readline and libedit.
- [ljlinenoise](https://luarocks.org/modules/fperrad/ljlinenoise) - a pure LuaJIT port of [linenoise](https://github.com/antirez/linenoise), a small alternative to readline and libedit.
- [LTUI](https://github.com/tboox/ltui) - A cross-platform terminal ui library based on Lua

### GUI
- [Yue](https://libyue.com/) - A library for creating native cross-platform GUI apps.
- [wxLua](http://wxlua.sourceforge.net/) - a wrapper around the [wxWidgets](http://www.wxwidgets.org/) cross-platform C++ GUI library.

### Debugging
- [MobDebug](https://github.com/pkulchenko/MobDebug) - Remote debugger for Lua.
- [clidebugger](https://github.com/ToddWegner/clidebugger) - A simple command line interface debugger for Lua 5.1 written in pure Lua.
- [inspect.lua](https://github.com/kikito/inspect.lua) - Human-readable representation of Lua tables
- [chrome-devtools-client](https://github.com/clear-code/lua-chrome-devtools-client) - Chrome DevTools client for Lua
- [lovebird](https://github.com/rxi/lovebird) - a Browser-based debug console. Originally made for LÖVE, but works in any project with LuaSocket support.
- **Profiling & Tracing**
  - [ProFi](https://github.com/mindreframer/ProFi.lua) - Simple profiler that works with LuaJIT and produces a report file.
  - [luatrace](https://github.com/geoffleyland/luatrace) - Toolset for tracing/analyzing/profiling script execution and generating detailed reports.
  - [StackTracePlus](https://github.com/ignacio/StackTracePlus) - Drop-in upgrade to Lua's stack traces which adds local context and improves readability.

### Testing
- [busted](http://olivinelabs.com/busted/) - BDD-style unit testing framework with great docs and Moonscript support.
- [LuaUnit](https://github.com/bluebird75/luaunit) - a popular unit-testing framework for Lua, with an interface typical of xUnit libraries.
- [luassert](https://github.com/Olivine-Labs/luassert) - Assertion library extending Lua's built-in assertions.
- [Luacheck](https://github.com/mpeterv/luacheck) - A tool for linting and static analysis of Lua code.
- [LuaInspect](https://github.com/davidm/lua-inspect) - a tool that does Lua code analysis, with plugins for HTML and SciTE.
- [lualint](https://github.com/philips/lualint) - lua linter and static analysis of global variable

### Cryptographic
- [lua-argon2](https://github.com/thibaultCha/lua-argon2) - the Argon2 password hashing function. Compatible with Lua 5.x and LuaJIT.
- [PLC](https://github.com/philanc/plc) (Pure Lua Crypto) - A small collection of crpytographic functions, and related utilities, implemented in pure Lua (version 5.3 or above)
- [Luazen](https://github.com/philanc/luazen) - a small library with various encoding, compression and cryptographic functions. All the functions work on strings, there is no stream or chunked more complex interfaces.
- [luatweetnacl](https://github.com/philanc/luatweetnacl) - Lua binding to the NaCl ("Tweet" version) crypto library

### File System
- [luafilesystem](https://github.com/keplerproject/luafilesystem) - LuaFileSystem complements the set of file system functions offered by the standard Lua distribution.

### Network
- [lua-http](https://luarocks.org/modules/daurnimator/http) [[Video]](https://www.youtube.com/watch?v=OeABiyUlAao) - HTTP Library for Lua. Supports HTTP(S) 1.0, 1.1 and 2.0; client and server.
- [lua-httpclient](https://github.com/lusis/lua-httpclient) - a unified wrapper around a ``openresty/ngx.location.capture`` or ``luasocket`` and ``luasec`` as drivers.
- [lua-websockets](https://github.com/lipp/lua-websockets) - This project provides Lua modules for Websocket Version 13 conformant clients and servers.
- [Lua-cURLv3](https://github.com/Lua-cURL/Lua-cURLv3) - Lua binding to libcurl
- [Ratchet](https://ratchet.icgood.net/) - The purpose of the ratchet library is to provide in Lua an asynchronous socket control mechanism for large numbers of sockets without using OS-level threads or losing the ease of synchronous socket programming.
- [Turbo](https://github.com/kernelsauce/turbo) - a asynchronous networking suite and framework built for LuaJIT 2 to building fast and scalable network applications. It uses a event-driven, non-blocking, threadless design.
- [lua-handlers](https://github.com/Neopallium/lua-handlers) - Provides a set of async. callback based handlers for working with raw TCP/UDP socket, ZeroMQ sockets, or HTTP client/server. You can get node.js style non-blocking IO with lua-handlers.
- [LuaSocket](https://luarocks.org/modules/luarocks/luasocket) [[Doc]](https://htmlpreview.github.io/?https://raw.githubusercontent.com/diegonehab/luasocket/master/doc/index.html) - Network support for the Lua language
- [lsocket](https://luarocks.org/modules/gunnar_z/lsocket) - simple and easy socket support for lua.
- [llsocket](https://luarocks.org/modules/mah0x211/llsocket) - low-level socket module [this module is under heavy development]
- [lua-resty-socket](https://luarocks.org/modules/thibaultcha/lua-resty-socket) - A module offering interoperability between the LuaSocket and cosocket APIs
- [lua-net](https://luarocks.org/modules/rayaman/lua-net) - Lua networking library that wraps around lua-socket to make networking easy.
- [dromozoa-socks](https://luarocks.org/modules/moyu/dromozoa-socks) - Toolkit for network and I/O programming

### Message broker / queues
- [lua-zmq](https://github.com/Neopallium/lua-zmq) - a library which extends the standard socket interfaces with an abstraction of asynchronous message queues. Lua bindings to ZeroMQ version 2.1, 2.2 or 3.2.
- [lzmq](https://github.com/zeromq/lzmq) - Lua binding to ZeroMQ version 3.2 or 4.x library. This library has C and FFI version of binding.

### Database drivers
- File systems (CVS, JSON formatted data, Flat-file database)
  > For a small database. The file is simple. A flat file can be a plain text file, or a binary file.
  > Records follow a uniform format, and there are no structures for indexing or recognizing relationships between records. Relationships can be inferred from the data in the database.
- Relational databases 
  > for features that provide consistency and reliability.
  - [LuaSQL](http://keplerproject.github.io/luasql/) - a simple interface from Lua to various DBMS. Connect to ODBC, ADO, Oracle, MySQL, SQLite, Firebird and PostgreSQL databases.
  - [LuaDBI](https://github.com/mwild1/luadbi) - Multi-backend SQL database interface library for Lua. It is designed to provide a RDBMS agnostic API. Supports DB2, Oracle, MySQL, PostgreSQL and SQLite databases with native database drivers.
  - [LuaSQLite3](http://lua.sqlite.org) - a Lua wrapper for the SQLite3 library.
  - [PL/Lua](https://github.com/pllua/pllua) - an implementation of Lua as a loadable procedural language for PostgreSQL.
  - [pgmoon](https://github.com/leafo/pgmoon) - a PostgreSQL client library written in Lua for OpenResty
- NoSQL databases
  > for high performance, high scalability and ease of access
  - [Tarantool](https://github.com/tarantool/tarantool) - is an in-memory database and application server.
  - [Redis](https://github.com/nrk/redis-lua) - A Lua client library for the Redis key value storage system.
  - [lredis](https://github.com/daurnimator/lredis) - a Redis (in-memory data structure store) client library for Lua

### Multitasking
**Native OS threads**:
> [Threads](https://en.wikipedia.org/wiki/Thread_(computing)) use [preemptive multitasking](https://en.wikipedia.org/wiki/Preemption_(computing)#Preemptive_multitasking).
  - [lua-llthreads](https://github.com/Neopallium/lua-llthreads) - Low-Level threads (pthreads and WIN32 threads) for Lua.
  - [lua-llthreads2](https://github.com/moteus/lua-llthreads2) - drop-in replacement for ``lua-llthreads`` library with several additional functionality.
  - [luaproc](https://github.com/askyrme/luaproc) [[paper]](http://www.inf.puc-rio.br/~roberto/docs/ry08-05.pdf) - multi-threading library. Message-passing model which allows multiple threads per OS thread.
  - [Lua Lanes](https://github.com/LuaLanes/lanes) - a lightweight, native, lazy evaluating multithreading library for Lua 5.1 to 5.4. Library implementing a message passing model with one OS thread per Lua thread.
  - [ltask](https://github.com/cloudwu/ltask) - lua multi task library, use n os thread for m lua states.
  - [Effil](https://github.com/effil/effil) [[slideshow]](http://www.lua.org/wshop18/Kupriyanov.pdf) - Multithreading support for Lua. It allows to spawn native threads and safe data exchange.

**Coroutine-based multitasking**:
> Lua uses [coroutines](https://en.wikipedia.org/wiki/Coroutine), non-preempted form of [concurrency](https://en.wikipedia.org/wiki/Concurrent_computing) known as [cooperative multitasking](https://en.wikipedia.org/wiki/Cooperative_multitasking). This means that coroutines provide concurrency but not [parallelism](https://en.wikipedia.org/wiki/Parallel_computing).
  - [Copas](https://luarocks.org/modules/tieske/copas) - Dispatcher based on coroutines that can be used for asynchronous networking. (It uses LuaSocket for TCP/IP stack and LuaSec for SSL support)
  - [Lumen](https://github.com/xopxe/Lumen) - Simple concurrent task scheduling.
  - Continuation Queues: [cqueues](https://luarocks.org/modules/daurnimator/cqueues) - Embeddable asynchronous networking, threading, and notification framework for Lua on Unix. Library for managing sockets, signals, and threads based on an event loop with coroutines.
  - [Coil](https://github.com/rxi/coil) - A tiny cooperative threading module for Lua.

> See this [comparison of options](http://lualanes.github.io/lanes/comparison.html) for more on the differences (particularly between ``lanes`` and ``luaproc``).
>
> See this [lua-users: MultiTasking](http://lua-users.org/wiki/MultiTasking) for links related to multitasking / multithreading / parallelization in Lua.

### Native OS APIs
- **POSIX**
  - [luaposix](https://luarocks.org/modules/gvvaughan/luaposix) - Lua bindings for POSIX APIs.

- **Windows-specific**
  - [winapi](https://github.com/stevedonovan/winapi) - Minimal Windows API
  - [lua-win32lib](https://github.com/bosorioo/lua-win32lib) - Small lib exposing some Win32 API to lua
  - [w32wrappers](https://github.com/luaforge/w32wrappers) - Wrappers for Win32 API functions & constants. 
  - [win32_api_luajit](https://github.com/rmbishop/win32_api_luajit) - Cosmin's win32 api for luajit (with adjustments) 
  - [luapower/winapi](https://luapower.com/winapi) - Windows, common controls and dialogs, message loop and system APIs for LuaJIT.

- **UNIX**
  - [ljsyscall](https://github.com/justincormack/ljsyscall) - Unix system calls for LuaJIT
  - [minisock](https://github.com/philanc/minisock) - a minimal Lua socket library for unix / tcp / udp connections. The API is very close to the standard Unix system calls.
  - [lunix](https://luarocks.org/modules/daurnimator/lunix) - Bindings to common Unix system APIs, striving for thread-safety.
  - [luaunix](https://luarocks.org/modules/mbalmer/luaunix) - A Lua Binding for Selected Unix functions and System Calls
  - [dromozoa-unix](https://luarocks.org/modules/moyu/dromozoa-unix) - Lua bindings for UNIX system interface

### Libraries
- [LuaWebDriver](https://github.com/clear-code/lua-web-driver) [[Blog]](https://www.clear-code.com/blog/2018/11/6.html) - a browser automation library using WebDriver API.
- [LuaCS](https://github.com/clear-code/luacs) [[Blog]](https://www.clear-code.com/blog/2018/5/23.html) - a CSS Selectors parser library for Lua
- [XMLua](https://github.com/clear-code/xmlua) [[Blog]](https://www.clear-code.com/blog/2017/12/25.html) - An user-friendly XML/HTML processing library for Lua based on libxml2
- [luaexpat](https://github.com/tomasguisasola/luaexpat) [[Doc]](https://matthewwild.co.uk/projects/luaexpat/) - a SAX XML parser based on the Expat (a stream-oriented XML parser) library.
  - [LuaExpatUtils](https://github.com/stevedonovan/LuaExpatUtils) - Utilities for working with LOM XML Documents
- [luapower/expat](https://github.com/luapower/expat) - A ffi binding for the Expat XML parser.
- [lua-cjson](https://github.com/mpx/lua-cjson) - Lua CJSON is a fast JSON encoding/parsing module for Lua
- [neturl](https://github.com/golgote/neturl) - A Robust URL Parser (with the ability to parse querystrings) and Builder for Lua.
- [lucihttp](https://github.com/jow-/lucihttp) - HTTP utility library with Lua binding9
- [LPeg](http://www.inf.puc-rio.br/~roberto/lpeg/) - a new pattern-matching library for Lua, based on Parsing Expression Grammars (PEGs). [[1]](http://www.inf.puc-rio.br/~roberto/docs/ry08-4.pdf) [[2]](http://www.inf.puc-rio.br/~roberto/docs/ry10-01.pdf)
  - [LPegLabel](https://github.com/sqmedeiros/lpeglabel) - a conservative extension of the ``LPeg`` library that provides an implementation of Parsing Expression Grammars (PEGs) with labeled failures.
  - [lpeg_patterns](https://github.com/daurnimator/lpeg_patterns) - A collection of LPEG patterns
- [lualinq](https://luarocks.org/modules/djfdyuruiry/lualinq) - Lightweight library which allows functional querying and transformation of lua arrays and objects
- [luatz](https://github.com/daurnimator/luatz) - Time, Date and Timezone library for lua
- [Libraries And Bindings](http://lua-users.org/wiki/LibrariesAndBindings) - a list of libraries implemented in Lua or implemented in another language (e.g. C) but having a Lua interface.

### Utilities
- [Allen](https://github.com/Yonaba/Allen) - An utility library to manipulate strings, which provides a set of helpers for strings operations for Lua.
- [Strictness](https://github.com/Yonaba/strictness) - a small module to track access and assignment to undefined variables in Lua
- [Serpent](https://github.com/pkulchenko/serpent) - Lua serializer and pretty printer.
- [lua-marshal](https://github.com/richardhundt/lua-marshal) - fast table serialization for Lua
- [base2base](https://github.com/catwell/base2base) - A pure Lua base-to-base converter
- [LuaTools](http://lua-users.org/wiki/LuaTools) - tools for use with Lua. Some of these tools written in Lua. 

### Miscellaneous
- [Luno](https://luarocks.org/modules/echiesse/luno) - General purpose libraries for Lua.
- [lua-stdlib](https://github.com/lua-stdlib/lua-stdlib/) - General Lua libraries
- [Penlight](https://github.com/stevedonovan/Penlight) - A set of pure Lua libraries focusing on input data handling, functional programming, and OS path management. Inspired by the Python standard libraries.
- [Microlight](https://github.com/stevedonovan/microlight) - A little library of useful Lua functions, intended as the 'light' version of Penlight
- [Carbon](https://github.com/lua-carbon/carbon) - a full suite intended to make Lua more semantic, expressive, and powerful. It aims to provide a set of functionality comparable to .NET, and runs on Lua 5.1 and LuaJIT on any platform.
- [lua-ext](https://github.com/andrew-d/lua-ext) - Standard library / extensions for Lua. math, operator functions, execution platform, Set implementation for Lua, I/O on strings; instead of files.
- [lua-apr](https://github.com/xolox/lua-apr) - Apache Portable Runtime binding for Lua. APR powers software  and makes the APR operating system interfaces available to Lua, serving as an extended standard library, focus in Threads, Processes, Directories.
- [lua-glib](https://bitbucket.org/darktjm/lua-glib/src/?at=master) [[Doc]](http://htmlpreview.github.io/?https://bitbucket.org/darktjm/lua-glib/raw/b8e99210f24587b25602009e575d70221552436e/lua-glib.html) - Yet another Lua-to-glib binding. This package wraps the GLib library fairly thinly. It is meant to be a portability and utility library.
- [LGI](https://luarocks.org/modules/pavouk/lgi) - Dynamic Lua binding to GObject-based libraries using [GObject-Instrospection](https://gi.readthedocs.io/). Allows using GObject-based libraries directly from Lua.
- [lgob](https://bitbucket.org/lucashnegri/lgob) - lgob provides bindings of GObject-based libraries (like GTK+ and WebKitGTK+), for Lua 5.1 / 5.2 / LuaJIT. It consists of a compiler that parses [GObject-Instrospection](https://gi.readthedocs.io/) [gir files](https://github.com/gtk-rs/gir-files) and generates Lua modules.

### Projects
### Asynchronous I/O
- [Luvit](https://luvit.io/) - Lua + libUV + jIT = pure awesomesauce
  - [Luver](https://github.com/squeek502/luver) - a ``luvit`` without ``lit``.
- [LuaNode](https://github.com/ignacio/LuaNode) - Asynchronous I/O for Lua, using the [Reactor pattern](https://en.wikipedia.org/wiki/Reactor_pattern) like Node.js, EventMachine or Twisted.
- [node-lua](https://github.com/socoding/node-lua) - a runtime environment and server engine for lua-based scripting that runs on multi-core machines in a multi-threaded manner.
- [Node.lua](https://github.com/czanyou/node.lua.v1) - a Lua runtime environment that uses an event-driven, non-blocking I/O model like Node.js
- [Lua Corovel](https://github.com/dmccuskey/lua-corovel) - Asynchronous, event-loop development environment for Lua

### Web Browser
- [Luakit](https://luakit.github.io/) - A fast, extensible, and customizable web browser based on the WebKit web content engine and the GTK+ toolkit.

### Web Plataforms
- [OpenResty](https://github.com/openresty/openresty) - Turning Nginx into a Full-Fledged Scriptable Web Platform
  - [VeryNginx](https://github.com/alexazhou/VeryNginx) - a very powerful and friendly nginx which provide WAF, Control Panel, and Dashboards.
  - [Orange](https://github.com/sumory/orange) - A Gateway based on OpenResty (Nginx+lua) for API Monitoring and Management.
  - [OpenStar](https://github.com/starjun/openstar) - Lua WAF, Nginx+Lua, OpenResty, LuaJIT, WAF+, CDN
  - [nginx-lua-prometheus](https://github.com/knyar/nginx-lua-prometheus) - Prometheus metric library for Nginx written in Lua
- [algernon](https://github.com/xyproto/algernon) - Small self-contained web server with Lua, Markdown, QUIC, Redis and PostgreSQL support

### Web Frameworks
- [Lapis](http://leafo.net/lapis/) - A web framework for Lua or MoonScript, powered by OpenResty
- [Sailor](http://sailorproject.org/) - A Lua MVC web framework.
- [Ophal](https://ophal.org/) - The highly scalable Lua CMS/CMF and web platform
- [Orbit](http://keplerproject.github.io/orbit/) - an MVC web framework for Lua, based on WSAPI. [[1]](https://luanova.org/orbit1-2/)
- [Lor Framework](http://lor.sumory.com/) - a fast, minimalist Web & API framework for lua based on OpenResty
- [Vanilla](https://github.com/idevz/vanilla) - An OpenResty Lua MVC Web Framework

### Game Framework
- [Skynet](https://github.com/cloudwu/skynet) - a lightweight online game framework which can be used in many other fields.
- [NoobHub](https://github.com/Overtorment/NoobHub) - Network multiplayer and messaging for CoronaSDK, Moai, Gideros, LÖVE & Defold

### Scientific Computing
- [Torch](http://torch.ch/) - a scientific computing framework with wide support for machine learning algorithms that puts GPUs first.
- [SciLua](http://scilua.org/) - A complete framework for numerical computing based on LuaJIT

### Digital Signal processing
- [LuaRadio](http://luaradio.io/) - a lightweight, embeddable flow graph signal processing framework for software-defined radio. It provides a suite of source, sink, and processing blocks, with a simple API for defining flow graphs, running flow graphs, creating blocks, and creating data types.

### Miscellaneous
- [Kong](https://github.com/Kong/kong) - a cloud-native, fast, scalable, and distributed Microservice Abstraction Layer (also known as an API Gateway, API Middleware or in some cases Service Mesh).
- [Snabb Switch](https://github.com/snabbco/snabb) - a simple and fast packet networking toolkit.
- [Telize](https://github.com/fcambus/telize) - a High performance REST API built on Nginx and Lua allowing to get a visitor IP address and to query location information (IP Geolocation).
- [SILE](https://github.com/simoncozens/sile) - a typesetting system; its job is to produce beautiful printed documents. Conceptually, SILE is similar to [TeX](https://en.wikipedia.org/wiki/TeX).
- [MoonGen](https://github.com/emmericp/MoonGen) - a fully scriptable high-speed packet generator built on [DPDK](https://en.wikipedia.org/wiki/Data_Plane_Development_Kit) and LuaJIT.
- [Prosody](https://prosody.im/) IM Server - a server for Jabber/XMPP written in Lua.

-----------------

### Blogs / Sites
- [Lua.Space](http://lua.space/) [[RSS Feed]](http://feeds.feedburner.com/Luaspace) - The Lua Community Blog
- [lua nova](https://luanova.org/) - welcome to the moon

### Style Guides
- [Lua-users style guide](http://lua-users.org/wiki/LuaStyleGuide) - A general, high-level style guide; unopinionated, easily agreed on.
- [Olivine style guide](https://github.com/Olivine-Labs/lua-style-guide) - A more opinionated and specific, and therefore more rigorous, guide.

### Guides / Tutorials
- [Lecture Notes based on PiL](http://www.dcc.ufrj.br/~fabiom/lua/) - course notes based on Programming in Lua book
- [Lua-Users: Lua Tutorial](http://lua-users.org/wiki/LuaTutorial) - This tutorial is aimed at all newcomers to the language Lua. We start off with where to find relevant introductory material and then progress to using the language with tutorials in the [TutorialDirectory)](http://lua-users.org/wiki/TutorialDirectory).
- [Lua Short Reference](http://lua-users.org/wiki/LuaShortReference) - The Lua short reference provides a concise summary of the Lua 5.1 syntax and core libraries.
- [Devhints.io: Cheatsheet for Lua](https://devhints.io/lua)
- [TutorialsPoint.com: Lua Tutorial](https://www.tutorialspoint.com/lua/) - is designed for all those readers who are looking for a starting point to learn Lua. It has topics suitable for both beginners as well as advanced users.
- [Lua Tutorial | Novice Tutorial](http://www.runoob.com/lua/lua-tutorial.html) - Lua Application Scenario: Game development
Stand-alone application script, Web Application Script, Database extensions and add-ons such as MySQL Proxy and MySQL WorkBench, Security system; such as an intrusion detection system.
- [RIP Tutorial: Lua](https://riptutorial.com/lua) - Getting started with Lua
- [The.Lua.Tutorial](http://luatut.com/) - An Introduction to Lua and The Crash Course to Lua.
- [Lua Crash Course](http://www.coppeliarobotics.com/helpFiles/en/luaCrashCourse.htm) - Short crash course readover, or reference for when you forget the basics.
- [LuaGuide](https://github.com/davisdude/LuaGuide/blob/master/LuaGuide.md) - A guide to help people learn Lua
- [Lua Missions](https://github.com/kikito/lua_missions) - A series of 'Missions' to work through which are designed to teach aspects of Lua along the way.
- [Litt's Lua Laboratory](http://www.troubleshooters.com/codecorn/lua/index.htm) - The 10% you need -- for 90% of your work
- [Learn X in Y minutes: Where X=Lua](https://learnxinyminutes.com/docs/lua/) - Learn Lua in 15 Minutes
- [Lua for Programmers](http://ebens.me/2012/08/27/lua-for-programmers-part-1) - Language Essentials, Data and Standard Libraries, More Advanced Concepts and Tips and Tricks.
- [Phrogz: Learning Lua](http://phrogz.net/lua/index.html) - Learning Lua/From JS, Referenced Values, Metatables, and Simple Inheritance, and Pseudo-OOP Syntax and Scope.
- [Learn Lua from JavaScript](https://www.oreilly.com/learning/learn-lua-from-javascript-part-1-an-introduction-to-lua) - If you know JavaScript, learning Lua is a snap, as Tyler Neylon explains in this series
- [Learn Lua the Hard Way](http://www.phailed.me/2011/02/learn-lua-the-hard-way-1/) - a person has never programmed before at all

### Lua Workshop
- Lua Workshop 2016
  - [On the design of Lua](https://www.youtube.com/watch?v=QystqRlz6bw) - Roberto Ierusalimschy (PUC-Rio)
  - [Practical LPeg](http://www.lua.org/wshop16/Mitchell.pdf)
- Lua Workshop 2017
  - [Functions in Lua](http://lua.moscow/conf/2017-03-LuaInMoscow/index.html#roberto) - In this talk, we will discuss how the mechanism of first-class functions has impacted the design of Lua and will also glimpse at its implementation.
- [Roberto Ierusalimschy • Talks](http://www.inf.puc-rio.br/~roberto/talks/index.html)

### Articles
- [A Look at the Design of Lua](https://cacm.acm.org/magazines/2018/11/232214-a-look-at-the-design-of-lua/fulltext) - Communications of the ACM, 2018
- [Small is Beautiful: the Design of Lua](https://web.stanford.edu/class/ee380/Abstracts/100310.html) [[video]](https://www.youtube.com/watch?v=DQtRSJUiZUw) - Stanford EE 380: Computer Systems Colloquium (2010)
- [The H Speed Guide to Lua](http://www.h-online.com/open/features/The-H-Speed-Guide-to-Lua-1517427.html) - Why Lua?, Developing with Lua, A quick look at Lua code, Talking with a Lua user
- [How uses Coroutines for non-blocking I/O](http://leafo.net/posts/itchio-and-coroutines.html) - It uses coroutines for all asynchronous operations like database queries and HTTP requests.
- [lightweight concurrency in lua](http://wingolog.org/archives/2018/05/16/lightweight-concurrency-in-lua) - Implementing fibers and a scheduler with Lua's Coroutines
- [Why we rewrote Lua in JS](https://hackernoon.com/why-we-rewrote-lua-in-js-a66529a8278d) - Lua for the browser
- [Interfacing Lua with C](https://ciel.im/posts/interfacing-lua-with-c/) - Lua provides an interface allowing to call C functions in Lua environment.
- [Asynchronous and Event-driven Programming in Lua](https://ciel.im/posts/asynchronous_lua/) - This article demonstrates how to bind libuv API to Lua environment.
- [Port Lua to Web Environment using WebAssembly (Wasm)](https://ciel.im/posts/port-lua-to-web-environment/) - using emscripten to compile Lua
- [Implementing Proper Getter/Setters in Lua](http://ebens.me/post/implementing-proper-gettersetters-in-lua) - a class in Lua (OOP)
- [Linked Lists in Lua](http://ebens.me/post/linked-lists-in-lua) - an example of creating custom data structures in Lua
- [Hooks in Lua for AOP](https://gist.github.com/jcmoyer/5716720) - pre/post method hooks in Lua for AOP
- [Embeddable scripting with Lua](https://www.ibm.com/developerworks/linux/library/l-lua/index.html) - Lua offers high-level abstraction without losing touch with the hardware
- [Embed Lua for scriptable apps](https://www.ibm.com/developerworks/linux/library/l-embed-lua/index.html) - Incorporate application scripting using a small language built for the job
- [Lua states, threads, libraries and memory layout](http://www.thijsschreijer.nl/blog/?p=693) - Diagrams and explains some more advanced concepts of the Lua VM, particularly when interfacing with C.
- [Lua: Good, bad, and ugly parts](http://notebook.kulchenko.com/programming/lua-good-different-bad-and-ugly-parts) - A thorough summary of the good, different, bad, and ugly aspects of Lua 5.2, including many subtle quirks, by the author of ZeroBrane Studio.

### Publications and Researchs
- [The Implementation of Lua 5.0](https://www.lua.org/doc/jucs05.pdf) [[slides]](http://www.inf.puc-rio.br/~roberto/talks/lua5-imp.pdf) - discuss about the implementation of Lua 5.0: its register-based virtual machine, the new algorithm for optimizing tables used as arrays, the implementation of closures, and the addition of coroutines.
- [Programming with Multiple Paradigms in Lua](http://www.inf.puc-rio.br/~roberto/docs/ry09-03.pdf)
- [Coroutines in Lua](http://www.inf.puc-rio.br/~roberto/docs/corosblp.pdf)
- [Lua.org: Papers and theses](https://www.lua.org/papers.html)
- [Roberto Ierusalimschy • Publications](http://www.inf.puc-rio.br/~roberto/cvpub.html)
- [LabLua - Programming Language Research](http://www.lua.inf.puc-rio.br/publications.html)

### [Lua Technical Notes](https://www.lua.org/notes/)
- [LTN12: Filters sources and sinks](http://lua-users.org/wiki/FiltersSourcesAndSinks) - Filters, Sources, Sinks, and Pumps
- [LTN13: Finalized Exceptions](http://lua-users.org/wiki/FinalizedExceptions) - LuaSocket's exception handling is based on Finalized Exceptions whitepaper.

### Books
- [Programming in Lua (PiL)](http://www.lua.org/pil/) - Intro to all aspects of Lua programming, written by Lua's chief architect. The official book first edition was aimed at Lua 5.0, remains largely relevant and available online.
  - [Table of contents](http://www.inf.puc-rio.br/~roberto/book/contents.pdf) - Read the table of contents of first edition.
  - [Preface](http://www.inf.puc-rio.br/~roberto/book/preface.pdf) - Read the preface of first edition.
  - [Source Code of the examples](http://www.inf.puc-rio.br/~roberto/book/code.html) - Get the source code for some examples from the book.
- [Programming Gems](http://www.lua.org/gems/) - A collection of articles covering existing wisdom and practices on programming well in Lua, in a broad variety of use cases.
- [Lua Quick Reference](https://foicica.com/lua) - This book covers: Object-oriented programming with Lua. Creating and working with Lua and C Modules. Lua's standard library and its C API. Collaborative multi-threading in Lua and C. How to program in and embed Lua 5.1 through 5.3, by the creator of Textadept.
- [Wrox - Beginning Lua Programming](http://shop.oreilly.com/product/9780470069172.do) - This book is for beginning programmers, game developers, and web site developers who are interested in a introduction to programming.
- [Creating Solid APIs with Lua](http://lua-users.org/lists/lua-l/2017-09/msg00092.html) - Learn how you can build APIs by integrating the Lua and C programming languages.
- [Lua Programming](https://en.wikibooks.org/wiki/Lua_Programming) - A shorter overview of the language, up to date for Lua 5.2, and available online.

### Lua VM and Bytecode
- [A No-Frills Introduction to Lua 5.0 VM Instructions (NFI)](http://luaforge.net/docman/83/95/ANoFrillsIntroToLua5VMInstructions.pdf)
- [A No-Frills Introduction to Lua 5.1 VM Instructions (NFI)](http://luaforge.net/docman/83/98/ANoFrillsIntroToLua51VMInstructions.pdf)
- [Lua 5.2 Bytecode and Virtual Machine](http://files.catwell.info/misc/mirror/lua-5.2-bytecode-vm-dirk-laurie/lua52vm.html)
- [Lua 5.3 Bytecode Reference](https://the-ravi-programming-language.readthedocs.io/en/latest/lua_bytecode_reference.html)

### Glossaries
- [Lua 5.3 Glossary](https://rawgit.com/dlaurie/lua-notes/master/glossary.html) - A glossary of some essential Lua terms.

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
