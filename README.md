# drafts
handy things and drafts for myself


# remove zero size files
`find . -size 0 -delete`

# GCC Coverage report compilation flags
`CFLAGS="-fprofile-arcs -ftest-coverage" CXXFLAGS="-fprofile-arcs -ftest-coverage"`


# FFMPEG custom build
`./configure --disable-shared --disable-inline-asm --cc=/home/arash/AFLplusplus-3.11c/afl-clang-fast --cxx=/home/arash/AFLplusplus-3.11c/afl-clang-fast++`


# Token search
`grep -rnw arrays-str/ -e TOKEN`

# mon
```
cmake -DMANUAL_SUBMODULES=1 -DCMAKE_C_COMPILER=/home/arash/AFLplusplus/afl-clang-fast -DCMAKE_CXX_COMPILER=/home/arash/AFLplusplus/afl-clang-fast++ ..

cmake -D STATIC=ON -D SANITIZE=ON -D BUILD_TESTS=ON -D USE_LTO=OFF -D CMAKE_C_COMPILER=/home/arash/AFLplusplus/afl-gcc -D CMAKE_CXX_COMPILER=/home/arash/AFLplusplus/afl-g++ -D ARCH="x86-64" -D CMAKE_BUILD_TYPE=fuzz -D BUILD_TAG="linux-x64" .




-DOSSFUZZ


cmake -DMANUAL_SUBMODULES=1 -D STATIC=ON -D SANITIZE=ON -D CMAKE_BUILD_TYPE=fuzz -DCMAKE_C_COMPILER=/home/arash/AFLplusplus/afl-clang-fast -DCMAKE_CXX_COMPILER=/home/arash/AFLplusplus/afl-clang-fast++ -D USE_LTO=OFF -DCMAKE_CXX_FLAGS="-fpic" -DCMAKE_C_FLAGS="-fpic" .
```
