
# Copyright 2019 Lawrence Livermore National Security. 
# Produced at the Lawrence Livermore National Laboratory.
# LLNL-CODE-781679. All Rights reserved. See file LICENSE for details.
#
# This file is part of graph-embed. For more information and source code
# availability, see github.com/LLNL/graph-embed
#
# SPDX-License-Identifier: LGPL-2.1

# Apply flags to all test targets
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED YES)
set(CMAKE_CXX_EXTENSIONS NO)

add_executable(embed embed.cpp)
target_link_libraries(embed partitioner)

add_executable(embedder embedder.cpp)
target_link_libraries(embedder partitioner)
