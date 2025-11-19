load("@rules_rust//rust:defs.bzl", "rust_library")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "monitor_rs",
    srcs = [
        "src/errors.rs",
        "src/lib.rs",
        "src/monitor.rs",
    ],
    deps = [
        "//health_monitor:hm_shared_lib",
        "@crates//:libc",
    ],
)
