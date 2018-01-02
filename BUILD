load("@io_bazel_rules_go//go:def.bzl", "go_prefix", "go_binary", "go_library")

go_prefix("test")

go_library(
    name = "go_default_library",
    srcs = ["test.go"],
    visibility = ["//visibility:private"],
)

go_binary(
    name = "test",
    embed = [":go_default_library"],
    visibility = ["//visibility:public"],
)
