package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["strategy.go"],
    tags = ["automanaged"],
    deps = [
        "//cmd/kube-aggregator/pkg/apis/apiregistration:go_default_library",
        "//cmd/kube-aggregator/pkg/apis/apiregistration/validation:go_default_library",
        "//pkg/api:go_default_library",
        "//pkg/fields:go_default_library",
        "//pkg/genericapiserver/api/request:go_default_library",
        "//pkg/labels:go_default_library",
        "//pkg/registry/generic:go_default_library",
        "//pkg/runtime:go_default_library",
        "//pkg/storage:go_default_library",
        "//pkg/util/validation/field:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//cmd/kube-aggregator/pkg/registry/apiservice/etcd:all-srcs",
    ],
    tags = ["automanaged"],
)