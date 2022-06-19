package(default_visibility = ["//visibility:public"])

py_binary (
    name = "main",
    srcs = glob(["main.py"]),
)

py_test(
    name = "test_main",
    srcs = ["test_main.py"],
    deps = ["main"],
)

test_suite(
    name = "all_tests",
    tests = [
        "test_main",
    ],
)

py_library(
    name = "test_lib",
    srcs = glob(["test*.py"]),
    deps = [
        "main",
    ],
)
