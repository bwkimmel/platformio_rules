package(
    default_visibility = ["//visibility:public"],
)

filegroup(
    name = "platformio_ini_tmpl",
    srcs = ["platformio.ini.tmpl"],
)

exports_files(["platformio.bzl"])

load("@platformio_python_deps//:requirements.bzl", "requirement")

py_binary(
    name = "pio",
    srcs = ["pio.py"],
    deps = [
        requirement("platformio"),
    ],
)
