# Inexor Reactive Graph Flow

| Project             | Module | Sub-Module | Functionality                                                        | Tests                                                                                                                                                      |
|---------------------|--------|------------|----------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Reactive Graph Flow | Plugin | Logical    | <img src="https://img.shields.io/badge/state-completed-brightgreen"> | [<img src="https://img.shields.io/codecov/c/github/aschaeffer/inexor-rgf-plugin-logical">](https://app.codecov.io/gh/aschaeffer/inexor-rgf-plugin-logical) |

### About Inexor

<a href="https://inexor.org/">
<img align="right" width="200" height="200" src="https://raw.githubusercontent.com/aschaeffer/inexor-rgf-plugin-logical/main/docs/images/inexor_2.png">
</a>

* Inexor will be a new first-person shooter game which is based on a new octree-based game engine.
* Inexor focuses on classic gameplay as we've seen in Cube2 or the Quake series.
* Inexor will be written from ground up new in C++17 and Rust.
* You can contribute anything you want: code, content, ideas..
* Inexor and all its content is 100% open source!

### About Inexor Reactive Graph Flow

The Inexor Reactive Graph Flow (RGF) manages reactive flows based on a graph database. The main interface is GraphQL.

* Semantic: Graph database with entities and relationships as first class citizens
* Reactive: entities and relationships are/can be reactive: If the input has been altered the entity processes its new state
* Interoperable: Use GraphQL for queries and mutations
* Extendable: Built in type system: components, entity types and relation types
* Memory efficient: Rust
* Fast: Rust
* Secure: Rust

### About this plugin

This plugin provides the type system and behaviour for logical operations.

[<img src="https://img.shields.io/badge/Language-Rust-brightgreen">](https://www.rust-lang.org/)
[<img src="https://img.shields.io/badge/Platforms-Linux%20%26%20Windows-brightgreen">]()
[<img src="https://img.shields.io/github/workflow/status/aschaeffer/inexor-rgf-plugin-logical/Rust">](https://github.com/aschaeffer/inexor-rgf-plugin-logical/actions?query=workflow%3ARust)
[<img src="https://img.shields.io/github/last-commit/aschaeffer/inexor-rgf-plugin-logical">]()
[<img src="https://img.shields.io/github/languages/code-size/aschaeffer/inexor-rgf-plugin-logical">]()
[<img src="https://img.shields.io/codecov/c/github/aschaeffer/inexor-rgf-plugin-logical">](https://app.codecov.io/gh/aschaeffer/inexor-rgf-plugin-logical)

[<img src="https://img.shields.io/github/license/aschaeffer/inexor-rgf-plugin-logical">](https://github.com/aschaeffer/inexor-rgf-plugin-logical/blob/main/LICENSE)
[<img src="https://img.shields.io/discord/698219248954376256?logo=discord">](https://discord.com/invite/acUW8k7)

#### Platform Compatibility

| Platform | Compatibility |
|----------|---------------|
| Linux    | ✓             |
| MacOS    | ✓             |
| Windows  | ✓             |

#### Components

| Name              | Description | Properties | Data Type | Socket Type |
|-------------------|-------------|------------|-----------|-------------|
| logical_gate      |             | lhs        | bool      | input       |
|                   |             | rhs        | bool      | input       |
|                   |             | result     | bool      | output      |
| logical_operation |             | lhs        | bool      | input       |
|                   |             | result     | bool      | output      |
| condition         |             | condition  | bool      | input       |
|                   |             | result     | any       | output      |

#### Entity Types

| Name         | Components        | Description                                                                                                                              |
|--------------|-------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| and          | logical_gate      |                                                                                                                                          |
| nand         | logical_gate      |                                                                                                                                          |
| nor          | logical_gate      |                                                                                                                                          |
| not          | logical_operation |                                                                                                                                          |
| or           | logical_gate      |                                                                                                                                          |
| xnor         | logical_gate      |                                                                                                                                          |
| xor          | logical_gate      |                                                                                                                                          |
| trigger      | condition         | <ul><li>If condition is true, propagate payload to result</li></ul>                                                                      |
| if_then_else | condition         | <ul><li>If condition is true, propagate then_payload to result</li><li>If condition is false, propagate else_payload to result</li></ul> |

### Thanks to

* https://github.com/xd009642/tarpaulin
* https://codecov.io/

### Sponsors

|                                                                                                                                                                                                                               |           |                                                                   |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------|-------------------------------------------------------------------|
| <a href="https://www.jetbrains.com/?from=github.com/inexorgame"><img align="right" width="100" height="100" src="https://raw.githubusercontent.com/aschaeffer/inexor-rgf-plugin-logical/main/docs/images/icon_CLion.svg"></a> | JetBrains | Special thanks to JetBrains for providing us with CLion licenses! |
