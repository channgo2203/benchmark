## Build for QNX platforms

To build, from the outside the benmark directory, run the following commands

```
mkdir build && cd build

cmake -DCMAKE_TOOLCHAIN_FILE=../benchmark/cmake/qnx-aarch64.cmake -DBENCHMARK_ENABLE_GTEST_TESTS=OFF -DCMAKE_CROSSCOMPILING=ON -DRUN_HAVE_GNU_POSIX_REGEX=0 -DRUN_HAVE_STD_REGEX=0 -DRUN_HAVE_POSIX_REGEX=0 -DRUN_HAVE_STEADY_CLOCK=0 -DBENCHMARK_ENABLE_TESTING=false ../benchmark
```
