# Multipurpose Media Type Identifier, Version 1.0
## Purpose
The MMTI provides a way to identify data types without an extension, and to differentiate files with the same extension. One can only make so many recognisable extensions with 4 latin characters. Some data is not to be used as a file, but still needs a way to be identified.

## Format
An MMTI string takes the format of `category/type`. For example, a Lua script would be `application/lua`. A CPIO archive would be `archive/cpio`, etc. MMTI strings should only use US-ASCII characters.

## Unregistered MMTI strings
MMTI strings that aren't registered should prefix the type with `x-`, such as `application/x-zoryapkg`.

## Categories
As of Version 1.0, the following categories are available for use.
* *application* - Any type of format which is to be executed
* *archive* - Any type of format which is used to archive other files
* *media* - Any type of format which contains video or audio
* *model* - Any type of format which contains data used to construct a 3D model
* *text* - Any type of format which is used to transmit textual data
* *message* - Any type of format which is used to transmit data over a network
* *other* - Any type of format which is not covered in the other categories

# Registed MMTI types.
| MMTI type | Extensions | Registration date |
| --- | --- | --- |
| `application/lua` | `.lua` | 2019-7-30 |
| `application/lua-binary` | `.luac` | 2019-7-30 |
| `application/lua-assembly` | `.luas` | 2019-7-30 |
| `archive/binary-cpio` | `.bcpio`, `.cpio` | 2019-7-30 |
| `archive/urf` | `.urf` | 2019-7-30 |
| `media/dfpwm` | `.dfpwm` | 2019-7-30 |
| `text/txt` | `.txt` | 2019-7-30 |
| `application/json` | `.json` | 2019-7-30 |
| `application/lua-table` | *N/A* | 2019-7-30 |
| `text/ohml` | `.ohml` | 2019-7-30 |
