#
# Copyright (c) 2022 Nordic Semiconductor ASA
#
# SPDX-License-Identifier: LicenseRef-Nordic-5-Clause
#

cmake_minimum_required(VERSION 3.20.0)

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(sidewalk_test_storage_kv)

cmock_handle(${ZEPHYR_BASE}/include/zephyr/fs/nvs.h zephyr/fs)

# add test file
FILE(GLOB app_sources src/*.c)
target_sources(app PRIVATE ${app_sources})

# generate runner for the test
test_runner_generate(${app_sources})
