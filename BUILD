cc_library(
    name = "cmp_mem_access",
    srcs = [
        "cmp_mem_access.c",
        "cmp_mem_access.h",
    ],
    hdrs = ["cmp_mem_access.h"],
    include_prefix = "cmp_mem_access",
    visibility = ["//visibility:public"],
    deps = ["@ch_cvra_cmp//:cmp"],
)

cc_test(
    name = "unittest",
    size = "small",
    srcs = ["cmp_mem_access_test.cpp"],
    deps = [
        "cmp_mem_access",
        "@ch_cvra_cmp//:cmp",
        "@ch_cvra_test_runner//:main",
    ],
)

cc_test(
    name = "example",
    size = "small",
    srcs = ["example.c"],
    deps = [
        ":cmp_mem_access",
        "@ch_cvra_cmp//:cmp",
    ],
)
