cmake_minimum_required(VERSION 3.18.0)

set(CMAKE_CXX_STANDARD 17)
project(test)

include(FetchContent)
FetchContent_Declare(
  solidity
  GIT_REPOSITORY https://github.com/junaire/solidity.git
  GIT_TAG origin/fix-wrong-cmake-variable
)

FetchContent_MakeAvailable(solidity)

add_subdirectory(lib)
