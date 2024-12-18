# Copyright (c) 2020 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(nu-mpu6500 STATIC EXCLUDE_FROM_ALL)

target_include_directories(nu-mpu6500
    PUBLIC
        .
)

target_sources(nu-mpu6500
    PRIVATE
        mpu6500.cpp
)

target_link_libraries(nu-mpu6500 PUBLIC mbed-core-flags)
