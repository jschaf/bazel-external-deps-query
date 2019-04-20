load("@io_bazel_rules_go//go:def.bzl", "go_binary")
load("@io_bazel_rules_go//proto:def.bzl", "go_proto_library")

proto_library(
    name = "deps_proto",
    srcs = ["deps.proto"],
)

go_proto_library(
    name = "deps_go_proto",
    compilers = ["@io_bazel_rules_go//proto:go_grpc"],
    importpath = "github.com/jschaf/bazel-external-deps-query",
    proto = ":deps_proto",
)
