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
