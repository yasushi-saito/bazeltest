workspace(name = "bazeltest")

# This works
# http_archive(
#     name = "io_bazel_rules_go",
#     sha256 = "76133849005134eceba9080ee28cef03316fd29f64a0a8a3ae09cd8862531d15",
#     strip_prefix = "rules_go-9cf23e2aab101f86e4f51d8c5e0f14c012c2161c",
#     urls = [
#         "https://github.com/bazelbuild/rules_go/archive/9cf23e2aab101f86e4f51d8c5e0f14c012c2161c.tar.gz",
#     ],
# )

# This is broken
http_archive(
   name = "io_bazel_rules_go",
   sha256 ="bad35f481c7ca1b3bb3e12d738dfd3f9318073a991fd50d8dc27dffb68b5e23a",
   strip_prefix = "rules_go-396f2424dd7c336e4b07b4f19d476f0749bc73dd/",
   urls = [
       "https://github.com/bazelbuild/rules_go/archive/396f2424dd7c336e4b07b4f19d476f0749bc73dd.tar.gz",
   ],
)
load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains")
go_rules_dependencies()
go_register_toolchains()
