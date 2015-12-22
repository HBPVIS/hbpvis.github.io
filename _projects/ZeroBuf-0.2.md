---
name: ZeroBuf
version: "0.2"
major: 0
minor: 2
description: Zero-copy, zero-serialize, zero-hassle protocol buffers
updated: 22/12/15
homepage: https://github.com/HBPVIS/ZeroBuf
repository: https://github.com/HBPVIS/ZeroBuf
issuesurl: https://github.com/HBPVIS/ZeroBuf
packageurl: 
license: LGPL
maturity: EP
maintainers: Human Brain Project (HBPVis@googlegroups.com)
contributors: Chevtchenko Grigori; Daniel Nachbaur; Raphael Dumusc; Stefan Eilemann
readmetype: text/x-markdown
---
ZeroBuf
=======

[TOC]

# Overview

ZeroBuf is a replacement for FlatBuffers, resolving the following
shortcomings:

* Direct get and set functionality on the defined data members
* A single, in-memory buffer storing all data members, which is directly
  serializable
* Usable, random access to the the data members
* Zero copy of the data used by the (C++) implementation from and to the network

# V1 Features

* Storage of (u)int[8,16,32,64,128]_t, float, double single elements, fixed
  size arrays and dynamic arrays
* Access to arrays using raw pointers, iterators, std::array,
  std::string and std::vector

# Extensions to flatbuffers grammar

* Arrays can have an optional fixed size specified as part of the type,
  e.g., ```matrix:[float:16]``` for a 16 value float array

