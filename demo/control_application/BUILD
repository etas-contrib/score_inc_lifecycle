cc_binary(
    name = "lmcontrol",
    srcs = [
        "control.hpp",
        "control_app_cli.cpp",
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
        "//external/ipc_dropin",
    ],
)

cc_binary(
    name = "control_daemon",
    srcs = [
        "control.hpp",
        "control_daemon.cpp",
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
        "//external/ipc_dropin",
        "//launch_manager:control_client",
        "//launch_manager:lifecycle_client",
    ],
)
