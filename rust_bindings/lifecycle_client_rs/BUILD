load("@rules_rust//rust:defs.bzl", "rust_library")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "lifecycle_client_rs",
    srcs = [
        "src/lib.rs",
        "src/lifecycle.rs",
    ],
    deps = [
        "//launch_manager:lifecycle_client",
        "@crates//:libc",
    ],
)
