# cpp-observe-proxy

Experimental third party proxy of the C++17 observer implementation from Lars.

## Usage

Generate the build files:

```console
❯ cmake -S . -B build
# ...
```

Build:

```console
❯ cmake --build build --parallel 2
[ 50%] Building CXX object CMakeFiles/observe_test.dir/main.cpp.o
[ 50%] Building CXX object examples/CMakeFiles/basic.dir/basic.cpp.o
[ 75%] Linking CXX executable basic
[ 75%] Built target basic
[100%] Linking CXX executable observe_test
[100%] Built target observe_test
```

Execute the tests:

```console
❯ build/observe_test
[doctest] doctest version is "2.4.4"
[doctest] run with "--help" for options
===============================================================================
[doctest] test cases: 3 | 3 passed | 0 failed | 0 skipped
[doctest] assertions: 3 | 3 passed | 0 failed |
[doctest] Status: SUCCESS!
```

Execute the basic example:

```console
❯ build/examples/basic
A triggered
B triggered with meaning of life and 42
I witness C with 123
I witness C with 234
I witness C with 1
I witness C with 2
I witness C with 42
```

## Status

Experimental.

**Note**: The default branch is `default`.
