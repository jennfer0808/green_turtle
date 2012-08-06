INCLUDE_DIRECTORIES(${CMAKE_SOURCE_DIR})

FILE(GLOB GREEN_TURTLE          *.h *.cc)
FILE(GLOB GREEN_TURTLE_NET      net/*.h net/*.cc)

SOURCE_GROUP(""         FILES ${GREEN_TURTLE})
SOURCE_GROUP("net"      FILES ${GREEN_TURTLE_NET})


ADD_LIBRARY(green_turtle STATIC
    ${GREEN_TURTLE}
    ${GREEN_TURTLE_NET})