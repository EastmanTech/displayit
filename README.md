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

<!-- ### <a href="todo">Homepage</a>

### <a href="todo">Demo</a> -->

## Nomenclature
> The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",<br>
> "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to<br>
> be interpreted as described in <a href="https://www.rfc-editor.org/rfc/rfc2119">RFC 2119</a>.

I use <a href="https://en.wikipedia.org/wiki/Backus%E2%80%93Naur_form">Backus-Naur Form</a>
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

<br>

## Dependencies
*todo*

<br>

## Configure and Build

```sh
cmake -B build -S . <config_options>  // configure
cmake --build build <build_options>   // build
```
where
```sh
<config_options> ::= <config_option>
                   | <config_option> <config_options>
                   | e

<config_option> ::= '-DCMAKE_BUILD_TYPE='<build_type>
                  | '-DBUILD_SHARED_LIBS='<shared_libs>

<build_options> ::= <build_option>
                  | <build_option> <build_options>
                  | e

<build_option> ::= '--config '<build_type>
                 | '--target '<target>

<build_type> ::= 'Release' | 'Debug' | 'MinSizeRel' | 'RelWithDebInfo'

<shared_libs> ::= 'On' | 'Off'

<target> ::= 'displayit' | 'install' | 'test'
```

## Usage
```sh
todo
```

## Run tests
```sh
cmake --build build --target test
```

## Developer Guide
In addition, the
<a href="https://www.boost.org/doc/libs/1_34_0/more/lib_guide.htm">Boost library requirements</a>
and guidelines MAY be used to<br>
guide the creation of the library. The following lists specific rules from that<br>
document which apply to this project. For rationale's on these decisisons, see<br>
the original text.

**One or more of these points may be modified from the original text of the<br>
document:**
<ul>
<li> Aim first for clarity and conciseness; optimization should be only a<br>
secondary concern

<li> Aim for ISO Standard C++. Than means making effective use of the<br>
standard features of the language, and avoiding non-standard compiler<br>
extensions. It also means using the C++ Standard Library where applicable.

<li> Headers should be good neighbors. See the
<a href="https://www.boost.org/doc/libs/1_34_0/more/header.htm">header policy</a>
<br> (^ With the exception of `boost/config.hpp` and Boost directory names)

<li> Use the naming conventions of the C++ Standard Library<br>
(See <a href="https://www.boost.org/doc/libs/1_34_0/more/lib_guide.htm#Naming">Naming conventions rationale</a>)

<li> Choose meaningful names - explicit is better than implicit, and readability<br>
counts. There is a strong preference for clear and descriptive names, even if<br>
lengthy.

<li> Use exceptions to report errors where appropriate, and write code that is<br>
safe in the face of exceptions.

<li> Avoid exception-specifications. See
<a href="https://www.boost.org/doc/libs/1_34_0/more/lib_guide.htm#Exception-specification">exception-specification rationale</a>.

<li> Provide sample programs or confidence tests so potential users can see how<br>
to use your library.

<li> Use fixed-width fonts.  See fonts rationale.

<li> Use spaces rather than tabs. See tabs rationale.

<li> Limit line lengths to 80 characters.

<li> Begin all source files (including programs, headers, scripts, etc.) with:<br>
<ul>
    <li> A comment line describing the contents of the file.
    <li> Comments describing copyright and licensing
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

## Author

**Alex Eastman**
<!-- * Twitter: [@-](https://twitter.com/-) -->

* Website: https://alexeastman.dev
* Github: [@alexeast99](https://github.com/alexeast99)
* LinkedIn: [@alexeast99](https://linkedin.com/in/alexeast99)

<!--
## Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check <a href="todo">issues page</a>. You can also take a look at the <a href="todo">contributing guide</a>.-->

## License

Copyright © 2022 <a href="https://github.com/alexeast99">Alex Eastman</a>.<br />
This project is <a href="https://unlicense.org">Unlicense</a> licensed.

***
_This README was generated by <a href="https://github.com/kefranabg/readme-md-generator">readme-md-generator</a>_