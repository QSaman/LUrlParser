project(LUrlParser) 
set(CMAKE_MINIMUM_VERSION 3.1)
cmake_minimum_required(VERSION ${CMAKE_MINIMUM_VERSION})

# Allow subfolders in solution file
set_property(GLOBAL PROPERTY USE_FOLDERS ON)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(SRC_LIB_LIST "LUrlParser.cpp")
add_library(${PROJECT_NAME} STATIC ${SRC_LIB_LIST})

install(TARGETS ${PROJECT_NAME} DESTINATION lib)
install(FILES LUrlParser.h DESTINATION include)
