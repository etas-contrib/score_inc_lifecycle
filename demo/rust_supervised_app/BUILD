load("@rules_rust//rust:defs.bzl", "rust_binary")

package(default_visibility = ["//visibility:public"])

rust_binary(
    name = "rust_supervised_app",
    srcs = [
        "src/main.rs",
    ],
    deps = [
        "//rust_bindings/lifecycle_client_rs",
        "//rust_bindings/monitor_rs",
        "@crates//:clap",
        "@crates//:libc",
        "@crates//:signal-hook",
    ],
)
