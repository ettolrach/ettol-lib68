# ettol-lib68

Standard types and functions missing from the regular GNU Algol 68 standard library.

These files are only intended to be used with GCC, no other Algol compilers are being used to test
the code.

# Compiling

The easiest way to use the module is to copy the source file, like "vendored" C code, or Rust
programs. Suppose you had a project with a `main.a68` which uses the module.

```a68
access Vector
begin
    puts("Hello, world!'n")
end
```

You would compile this by using the GCC compiler like so:

```
ga68 -c vector.a68 && ga68 -c main.a68 && ga68 vector.o main.o -o ./main`
```

This will be familiar with users of the GCC compiler, e.g. for C programs. For more help, see [§
2.2.4 *Modules and exports* in the GNU Algol 68 compiler
manual](https://gcc.gnu.org/onlinedocs/ga68/Modules-and-exports.html#Modules-and-exports-1).

# Licence

Copyright 2026 ettolrach

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
