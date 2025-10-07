cmake_minimum_required(VERSION 4.0)
project(Pendulum_C C)

set(CMAKE_C_STANDARD 11)

add_executable(Pendulum_C
    src/main.c
    src/libraries/loging_bfo/log.c
    src/libraries/loging_bfo/log.h
    src/libraries/string_bfo/String_array_struct.c
    src/libraries/string_bfo/String_struct.c
    src/libraries/string_bfo/String_struct.h
    src/libraries/string_bfo/String_struct_formatting.c
    src/libraries/terminal_bfo/colors_bfo/bins.c
    src/libraries/terminal_bfo/colors_bfo/bins.h
    src/libraries/terminal_bfo/colors_bfo/colors.c
    src/libraries/terminal_bfo/colors_bfo/colors.h
    src/libraries/terminal_bfo/progress_bar/progres_bar.c
    src/libraries/terminal_bfo/progress_bar/progres_bar.h
    src/libraries/terminal_bfo/terminal_funcs.h
    src/libraries/tests_bfo/test_funcs.c
    src/libraries/tests_bfo/test_funcs.h)

target_link_libraries(Pendulum_C m)
