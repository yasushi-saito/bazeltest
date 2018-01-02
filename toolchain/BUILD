package(default_visibility = ["//visibility:public"])

filegroup(
    name = "cc_wrapper",
    srcs = ["cc_wrapper.sh"],
)

cc_toolchain_suite(
    name = "toolchain",
    toolchains = {
        "k8|compiler": ":cc-gcc-k8",
    },
)

cc_toolchain(
    name = "cc-gcc-k8",
    all_files = ":cc_wrapper",
    compiler_files = ":empty",
    cpu = "local",
    dwp_files = ":empty",
    dynamic_runtime_libs = [":empty"],
    linker_files = ":empty",
    objcopy_files = ":empty",
    static_runtime_libs = [":empty"],
    strip_files = ":empty",
    supports_param_files = 1,
)
