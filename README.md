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

# Legal License

Licesned under the BSD 4-Clause License

Copyright 2026, Float314 and contributors.

Licensed under the Berkeley Software Distribution License, BSD 4-Clause
License (the "License"); you may not use this file except in compliance with
the License. You may obtain a copy of the License at

https://choosealicense.com/licenses/bsd-4-clause/

THIS SOFTWARE IS PROVIDED BY COPYRIGHT HOLDER "AS IS" AND ANY EXPRESS OR
IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
EVENT SHALL COPYRIGHT HOLDER BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.