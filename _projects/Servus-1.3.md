---
name: Servus
version: "1.3"
major: 1
minor: 3
description: C++ network oriented utilities including a zeroconf implementation
updated: 01/06/16
homepage: https://github.com/HBPVIS/Servus
repository: https://github.com/HBPVIS/Servus.git
issuesurl: https://github.com/HBPVIS/Servus/issues
packageurl: 
license: 
maturity: EP
maintainers: Human Brain Project (HBPVis@googlegroups.com)
contributors: hernando
readmetype: text/x-markdown
---
[TOC]

# Introduction {#Introduction}

Servus is a small C++ network utility library that provides a zeroconf
API, URI parsing and UUIDs.

Servus 1.2 can be retrieved by cloning the
[source code](https://github.com/HBPVIS/servus). Please file a
[Bug Report](https://github.com/HBPVis/servus/issues) if you find any issues
with this release.

## Features {#Features}

Servus provides classes for:

* 128 bit UUIDs
* An URI class to parse strings using generic syntax from
  [RFC3986](https://www.ietf.org/rfc/rfc3986.txt)
* Zeroconf announcement and browsing using Avahi or DNSSD
* Detailed @ref Changelog

# Building {#Building}

Servus is a cross-platform library, the only mandatory dependency is a
C++11 compiler. Zeroconf will be available in those platforms were
either Avahi or DNSSD are available, otherwise an empty dummy backend is
used. Servus uses CMake to provide a platform-independent build
configuration. The following platforms and build environments have been
tested:

* Linux: Ubuntu 14.04, RHEL 6 using gcc 4.8.2
* Windows: 8 using Visual Studio 12
* Mac OS X: 10.9 and 10.10 using clang 6

The following external, pre-installed optional dependencies are used:

* Boost.Test to build unit tests
* Avahi (avahi-client) or DNSSD (Apple Bonjour) for zeroconf
* Qt5 Core for servus::qt::ItemModel
* Qt5 Widgets for servusBrowser tool

Building from source is as simple as:

    git clone https://github.com/HBPVIS/Servus.git
    mkdir Servus/build
    cd Servus/build
    cmake ..
    make

