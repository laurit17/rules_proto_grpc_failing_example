package(default_visibility = ["//visibility:public"])

load("@rules_proto_grpc//python:defs.bzl", "python_proto_library")

proto_library(
  name = "a_proto",
  srcs = ["a.proto"],
)

cc_proto_library(
  name = "a_cc_proto",
  deps = [":a_proto"],
)

python_proto_library(
  name = "a_py_proto",
  deps = [":a_proto"],
)

proto_library(
  name = "b_proto",
  srcs = ["b.proto"],
  deps = [":a_proto"],
)

cc_proto_library(
  name = "b_cc_proto",
  deps = [":b_proto"],
)

python_proto_library(
  name = "b_py_proto",
  deps = [":b_proto"],
)

proto_library(
  name = "c_proto",
  srcs = ["c.proto"],
)

python_proto_library(
  name = "c_py_proto",
  deps = [":c_proto"],
)
