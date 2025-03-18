
add_executable(top-movies   top-movies/main.cpp)
add_executable(word-frequency   word-frequency/main.cpp)


set_property(TARGET top-movies   PROPERTY FOLDER "examples/chapter-07")
set_property(TARGET word-frequency   PROPERTY FOLDER "examples/chapter-07")
