
add_executable(contained-type   contained-type/main.cpp)
add_executable(dsl   dsl/main.cpp)
add_executable(make-curried   make-curried/main.cpp)


set_property(TARGET contained-type   PROPERTY FOLDER "examples/chapter-11")
set_property(TARGET dsl   PROPERTY FOLDER "examples/chapter-11")
set_property(TARGET make-curried   PROPERTY FOLDER "examples/chapter-11")
