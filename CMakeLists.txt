cmake_minimum_required(VERSION 3.18.0)

set(CMAKE_CXX_STANDARD 17)
project(test)

include(FetchContent)
FetchContent_Declare(
  solidity
  GIT_REPOSITORY https://github.com/ethereum/solidity.git
  GIT_TAG v0.8.20
)

FetchContent_MakeAvailable(solidity)

add_subdirectory(lib)
