package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = ["hairpin.go"],
    tags = ["automanaged"],
    deps = [
        "//pkg/util/exec:go_default_library",
        "//vendor:github.com/golang/glog",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["hairpin_test.go"],
    library = "go_default_library",
    tags = ["automanaged"],
    deps = ["//pkg/util/exec:go_default_library"],
)
