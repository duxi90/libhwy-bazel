workspace(name = "libhwy-bazel")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "bazel_skylib",
    urls = ["https://github.com/bazelbuild/bazel-skylib/releases/download/0.9.0/bazel_skylib-0.9.0.tar.gz"],
)

http_archive(
    name = "rules_license",
    urls = [
        "https://github.com/bazelbuild/rules_license/releases/download/0.0.4/rules_license-0.0.4.tar.gz",
        "https://mirror.bazel.build/github.com/bazelbuild/rules_license/releases/download/0.0.4/rules_license-0.0.4.tar.gz",
    ],
    sha256 = "6157e1e68378532d0241ecd15d3c45f6e5cfd98fc10846045509fb2a7cc9e381",
)

libhwy_version = "1.0.4"
http_archive(
	name = "com_github_google_highway",
	urls = ["https://github.com/google/highway/archive/refs/tags/{}.zip".format(libhwy_version)],
	strip_prefix = "highway-{}".format(libhwy_version),
)

