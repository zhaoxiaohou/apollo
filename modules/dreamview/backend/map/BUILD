load("//tools:cpplint.bzl", "cpplint")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "map_service",
    srcs = [
        "map_service.cc",
    ],
    hdrs = [
        "map_service.h",
    ],
    deps = [
        "//modules/map/pnc_map",
        "//third_party/json",
        "@glog//:glog",
    ],
)

cc_test(
    name = "map_service_test",
    size = "small",
    srcs = [
        "map_service_test.cc",
    ],
    data = [
        "//modules/dreamview/backend/testdata",
    ],
    deps = [
        ":map_service",
        "@gtest//:main",
    ],
)

cpplint()
