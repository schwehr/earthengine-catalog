# Bazel workspace for the Earth Engine Catalog.

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "io_bazel_rules_jsonnet",
    sha256 = "c51ba0dba41d667fa5c64e56e252ba54be093e5ae764af6470dabca901f373eb",
    strip_prefix = "rules_jsonnet-0.5.0",
    urls = ["https://github.com/bazelbuild/rules_jsonnet/archive/0.5.0.tar.gz"],
)
load("@io_bazel_rules_jsonnet//jsonnet:jsonnet.bzl", "jsonnet_repositories")

jsonnet_repositories()

load("@google_jsonnet_go//bazel:repositories.bzl", "jsonnet_go_repositories")

jsonnet_go_repositories()

load("@google_jsonnet_go//bazel:deps.bzl", "jsonnet_go_dependencies")

jsonnet_go_dependencies()
