project(sgsmooth)

include_directories(include/sgsmooth)
add_definitions(-fPIC)
add_definitions(-std=c++11)
add_library(sgsmooth src/SGSmooth.cpp)

install (TARGETS sgsmooth DESTINATION lib)
install (DIRECTORY include/sgsmooth DESTINATION include)
