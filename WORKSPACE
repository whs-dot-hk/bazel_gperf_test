load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "rules_foreign_cc",
    strip_prefix = "rules_foreign_cc-master",
    url = "https://github.com/bazelbuild/rules_foreign_cc/archive/master.zip",
)

load("@rules_foreign_cc//:workspace_definitions.bzl", "rules_foreign_cc_dependencies")

rules_foreign_cc_dependencies()

http_archive(
    name = "gperf",
    build_file = "@//:BUILD.gperf",
    strip_prefix = "gperf-3.1",
    urls = ["https://ftp.gnu.org/pub/gnu/gperf/gperf-3.1.tar.gz"],
)
