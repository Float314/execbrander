# execbrand - CMake Executable brander

Embeds metadata.rc into executables and DLLs. Ex - 

```cmake
include(execbrand)

execbrand_embedrc(metadata.json)

```

And `metadata.json` - 
```json
{
    "name" : "xyz program",
    "legalCopyright": "Copyright (C) 2026, SomeCompany IT Tech. All rights reserved",
    "version" : "1.0.0.2",
    "description": "Some useful program :)"
}
```
thats it! 

# Why? 

Writing Windows resource metadata manually is annoying and isnt niche at all..

Traditional .rc files are:

- verbose
- outdated
- hard to maintain
- painful for simple projects
- Could've used INI or TOML Files tbh

execbrand provides a cleaner workflow using JSON and CMake.

# Recommended project structure

root
   \- src/ 
   \- config/ 
        \- metadata.json
    \- Other files

# Legal License

Licesned under the GNU GPL v3

    <one line to give the program's name and a brief idea of what it does.>
    Copyright (C) 2026, Float314

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>.


<img src="https://www.gnu.org/graphics/gplv3-with-text-136x68.png" alt="GNU GPL v3">