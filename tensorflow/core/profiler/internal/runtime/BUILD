package(
    default_visibility = ["//tensorflow:internal"],
)

licenses(["notice"])  # Apache 2.0

load(
    "//tensorflow:tensorflow.bzl",
    "tf_cuda_library",
)

tf_cuda_library(
    name = "eager_profiler",
    srcs = [
        "eager_profiler.cc",
    ],
    deps = [
        "//tensorflow/core/common_runtime/eager:context",
        "//tensorflow/core/profiler/internal:profiler_interface",
        # "//tensorflow/stream_executor/lib",
    ],
    alwayslink = True,
)
