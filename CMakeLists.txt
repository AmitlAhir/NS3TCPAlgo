# ##############################################################################
# Required CMake version            #
# ##############################################################################
cmake_minimum_required(VERSION 3.13..3.13)

# ##############################################################################
# Project name                        #
# ##############################################################################
project(NS3 Example)

# minimum compiler versions
set(AppleClang_MinVersion 11.0.0)
set(Clang_MinVersion 10.0.0)
set(GNU_MinVersion 9.0.0)

# common options
option(NS3_EXAMPLES "Enable examples to be built" ON)


# Build NS library examples
add_subdirectory(examples)

write_lock()
write_configtable()
