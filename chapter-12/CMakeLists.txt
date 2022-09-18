
add_executable(bookmark-service   bookmark-service/main.cpp)
add_executable(bookmark-service-with-reply   bookmark-service-with-reply/main.cpp)
target_include_directories(bookmark-service PRIVATE ${Boost_INCLUDE_DIRS})

set_property(TARGET bookmark-service   PROPERTY FOLDER "examples/chapter-12")
set_property(TARGET bookmark-service-with-reply   PROPERTY FOLDER "examples/chapter-12")
