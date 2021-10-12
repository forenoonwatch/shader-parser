# Shader Parser

## Description

A simple recursive descent parser to get important information out of a GLSL source file required by rendering engines. Currently only supports getting data associated with expressions prefixed by a layout qualifier, with the primary purpose currently being to get variable information from Uniform Buffers and Shader Storage Buffers.

Disclaimer: This is both incomplete and not fully representative of GLSL grammar. The primary purpose of this parser is to augment my personal rendering engine.

# Background

Originally written to get memory layout/type data from shader source files to integrate it into my game engine, but shortly after writing it I discovered the OpenGL API functions associated with fetching this information from the shaders in a much easier and stabler way.

# Building 

Requires GCC and GNU make, run `make` in the main directory

# Usage

Call `shader-parser file_name.glsl` and the program will print out information on variable qualifiers

