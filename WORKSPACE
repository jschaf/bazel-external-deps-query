load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

go_commit = "c6506a2734913a063b458896187c787eed00ca08"
http_archive(
    name = "io_bazel_rules_go",
    urls = ["https://github.com/bazelbuild/rules_go/archive/%s.tar.gz" % go_commit],
    strip_prefix = "rules_go-" + go_commit,
)
load("@io_bazel_rules_go//go:deps.bzl", "go_rules_dependencies", "go_register_toolchains")
go_rules_dependencies()
go_register_toolchains()

zlib_commit = "cacf7f1d4e3d44d871b605da3b647f07d718623f"
http_archive(
    name = "zlib",
    urls = ["https://github.com/madler/zlib/archive/%s.tar.gz" % zlib_commit],
    strip_prefix = "zlib-" + zlib_commit,
    build_file = "@//:zlib.BUILD",
)


protobuf_commit = "60b66a119d17f0a2a595a231bea87cd4f4cf2689"
http_archive(
    name = "com_google_protobuf",
    urls = ["https://github.com/protocolbuffers/protobuf/archive/%s.tar.gz" % protobuf_commit],
    strip_prefix = "protobuf-" + protobuf_commit,
)
