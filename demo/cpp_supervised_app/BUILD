cc_binary(
    name = "cpp_supervised_app",
    srcs = [
        "main.cpp",
    ],
    copts = select({
        "//config:x86_64-qnx": [],
        "//conditions:default": ["-pthread"],
    }),
    linkopts = select({
        "//config:x86_64-qnx": [],
        "//conditions:default": [
            "-lpthread",
            "-lrt",
        ],
    }),
    visibility = ["//visibility:public"],
    deps = [
        "//health_monitor:hm_shared_lib",
        "//launch_manager:lifecycle_client",
    ],
)
