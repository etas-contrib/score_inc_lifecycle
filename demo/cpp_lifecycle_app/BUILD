cc_binary(
    name = "cpp_lifecycle_app",
    srcs = [
        "main.cpp",
    ],
    copts = select({
        "//config:x86_64-qnx": [],
        "//conditions:default": ["-pthread"],
    }),
    linkopts = select({
        "//config:x86_64-qnx": [],
        "//conditions:default": ["-lpthread"],
    }),
    visibility = ["//visibility:public"],
    deps = [
        "//launch_manager:lifecycle_client",
    ],
)
