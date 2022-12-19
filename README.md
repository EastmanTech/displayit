<h1 align="center">Welcome to displayit</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-0.0.1-blue.svg?cacheSeconds=2592000" />
  <a href="todo" target="_blank">
    <img alt="Documentation" src="https://img.shields.io/badge/documentation-some-orange.svg" />
  </a>
  <a href="https://unlicense.org" target="_blank">
    <img alt="License: Unlicense" src="https://img.shields.io/badge/License-Unlicense-yellow.svg" />
  </a>
  <!-- <a href="https://twitter.com/-" target="_blank">
    <img alt="Twitter: -" src="https://img.shields.io/twitter/follow/-.svg?style=social" />
  </a> -->
</p>

A cross-platform, extensible, and fast library for displaying data at runtime.

<!-- ### [Homepage](todo)

### [Demo](todo) -->

## Nomenclature
> The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",<br>
> "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to<br>
> be interpreted as described in [RFC 2119](https://www.rfc-editor.org/rfc/rfc2119).

I use [Backus-Naur Form](https://en.wikipedia.org/wiki/Backus%E2%80%93Naur_form)
throughout this document. The terminal symbol<br>
*e* without quotes means "nothing", or the absence of something.

If the form I use in this document is confusing, I encourage you to submit<br>
an issue, and we can discuss how to make it more clear for everyone :-)

<br>

## Purpose
There are plenty of tools available for displaying data in C++. A short list:<br>

<li> <a href=https://github.com/alandefreitas/matplotplusplus>matplotplusplus</a>
<li> <a href=https://github.com/graphia-app/graphia>graphia</a>
<li> <a href=https://github.com/tbattz/openGLPlotLive>openGLPlotLive</a>

<br>

These tools are impressive and extensive, but they're also complex and require<br>
time to learn and use properly. This library trades extensibility and<br>
customizability for simplicity and ease of use. It might even serve as a<br>
prototyping library, until the user is ready to learn a more complex data<br>
visualization tool.

<br>

## Goals
<ul>
<li> MUST provide an API for users to display arbitrary data in a uniform and<br>
consistent manner
<li> MUST NOT add a significant burden to the maintenance or development of<br>
the program in which it is used
<li> MUST provide packages for installation (todo)
<li> MUST support C++17 and later
<li> SHOULD support C++11 and later
</ul>

## Dependencies
<li> [Ninja-Build](https://ninja-build.org/)

## Installation
### Windows
*todo*

### Linux
*todo*

### MacOS
*todo*

## Developer Guide
In addition, the
[Boost library requirements](https://www.boost.org/doc/libs/1_34_0/more/lib_guide.htm)
and guidelines MAY be used to<br>
guide the creation of the library. The following lists specific rules from that<br>
document which apply to this project. For rationale's on these decisisons, see<br>
the original text.

**One or more of these points may be modified from the original text of the<br>
document:**
<ul>
<li> Aim first for clarity and conciseness; optimization should be only a<br>
secondary concern ...

<li> Aim for ISO Standard C++. Than means making effective use of the<br>
standard features of the language, and avoiding non-standard compiler<br>
extensions. It also means using the C++ Standard Library where applicable.

<li> Headers should be good neighbors. See the
[header policy](https://www.boost.org/doc/libs/1_34_0/more/header.htm) ...
<br> (^ With the exception of `boost/config.hpp` and Boost directory names)

<li> Use the naming conventions of the C++ Standard Library<br>
(See [Naming conventions rationale](https://www.boost.org/doc/libs/1_34_0/more/lib_guide.htm#Naming)) ...

<li> Choose meaningful names - explicit is better than implicit, and readability<br>
counts. There is a strong preference for clear and descriptive names, even if<br>
lengthy.

<li> Use exceptions to report errors where appropriate, and write code that is<br>
safe in the face of exceptions.

<li> Avoid exception-specifications. See
[exception-specification rationale](https://www.boost.org/doc/libs/1_34_0/more/lib_guide.htm#Exception-specification).

<li> Provide sample programs or confidence tests so potential users can see how<br>
to use your library.

<li> Use fixed-width fonts.  See fonts rationale.

<li> Use spaces rather than tabs. See tabs rationale.

<li> Limit line lengths to 80 characters.

<li> Begin all source files (including programs, headers, scripts, etc.) with:<br>
<ul>
    <li> A comment line describing the contents of the file.
    <li> Comments describing copyright and licensing ...
</ul>

<li> Directory naming:
<ul>
    <li> Contains only lowercase ASCII letters, numbers, and underscores
    <li> Leading character must be alphabetic
    <li> Maximum length of 31 characters
</ul>

<li> File naming:
  - Files intended to be processed by a C++ compiler as part of a<br>
translation unit should have a three-letter filename extension ending in<br>
"pp"
  - Other files should not use extensions ending in "pp"
</ul>

<br>

## Configure and Build

```sh
cmake -B build -S . <options>
cmake --build build --target <target>
```
where
```sh
<options> ::= <option>
            | <option> <options>
            | e

<option> ::= '-DCMAKE_BUILD_TYPE='<build-type>
            | '-DBUILD_SHARED_LIBS='<shared-libs>

<build-type> ::= 'Release' | 'Debug' | 'MinSizeRel' | 'RelWithDebInfo'

<shared-libs> ::= 'On' | 'Off'

<target> ::= 'displayit'
```

## Usage

```sh
todo
```

## Run tests

```sh
todo
```

## Author

**Alex Eastman**
<!-- * Twitter: [@-](https://twitter.com/-) -->

* Website: https://alexeastman.dev
* Github: [@alexeast99](https://github.com/alexeast99)
* LinkedIn: [@alexeast99](https://linkedin.com/in/alexeast99)

<!--
## Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check [issues page](todo). You can also take a look at the [contributing guide](todo).-->

## License

Copyright © 2022 [Alex Eastman](https://github.com/alexeast99).<br />
This project is [Unlicense](https://unlicense.org) licensed.

***
_This README was generated by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_