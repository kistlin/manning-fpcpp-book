
add_executable(functors-optional   functors-optional/main.cpp)
add_executable(monad-optional   monad-optional/main.cpp)
add_executable(monad-range   monad-range/main.cpp)
add_executable(monad-vector   monad-vector/main.cpp)


set_property(TARGET functors-optional   PROPERTY FOLDER "examples/chapter-10")
set_property(TARGET monad-optional   PROPERTY FOLDER "examples/chapter-10")
set_property(TARGET monad-range   PROPERTY FOLDER "examples/chapter-10")
set_property(TARGET monad-vector   PROPERTY FOLDER "examples/chapter-10")
