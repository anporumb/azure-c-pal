#Copyright (c) Microsoft. All rights reserved.
#Licensed under the MIT license. See LICENSE file in the project root for full license information.

set(theseTestsName uniqueid_ut)

set(uniqueid_ut_test_file ${theseTestsName}_linux.c)

set(${theseTestsName}_test_files
    ${uniqueid_ut_test_file}
)


set(${theseTestsName}_c_files
    ../../src/uniqueid_linux.c
)

set(${theseTestsName}_h_files
    ../../../interfaces/inc/c_pal/uniqueid.h
)

build_test_artifacts(${theseTestsName} "tests/c_pal" ADDITIONAL_LIBS pal_interfaces uuid)

