package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "attention_notify.go",
        "common.go",
        "roominfo_notify.go",
        "service.go",
        "uname_notify.go",
    ],
    importpath = "go-common/app/job/live/push-search/service",
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
    deps = [
        "//app/job/live/push-search/conf:go_default_library",
        "//app/job/live/push-search/dao:go_default_library",
        "//app/job/live/push-search/model:go_default_library",
        "//app/service/live/relation/api/liverpc/v1:go_default_library",
        "//app/service/live/room/api/liverpc/v1:go_default_library",
        "//app/service/live/room/api/liverpc/v2:go_default_library",
        "//app/service/live/user/api/liverpc/v3:go_default_library",
        "//app/service/main/account/api:go_default_library",
        "//library/log:go_default_library",
        "//library/net/rpc/liverpc/context:go_default_library",
        "//library/queue/databus:go_default_library",
        "//library/sync/errgroup:go_default_library",
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
        "//app/job/live/push-search/service/migrate:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
