load("//tensorflow/tsl/platform:rules_cc.bzl", "cc_library")
load("//tensorflow/compiler/xla/mlir/backends/openxla:build_config.bzl", "if_openxla")

package(
    # copybara:uncomment default_applicable_licenses = ["//tensorflow:license"],
    default_visibility = ["//tensorflow/compiler/xla:internal"],
    licenses = ["notice"],
)

# copybara:uncomment_begin(not supported in OSS build)
#
# cc_library(
#     name = "de_bufferization",
#     hdrs = if_openxla(["de_bufferization.h"]),
#     deps = [
#         "@llvm-project//llvm:Support",
#         "@llvm-project//mlir:IR",
#         "@llvm-project//mlir:MemRefDialect",
#     ],
# )
#
# cc_library(
#     name = "convert_compiled_ops",
#     srcs = if_openxla(["convert_compiled_ops.cc"]),
#     hdrs = if_openxla(["convert_compiled_ops.h"]),
#     # TODO(ezhulenev): Override cc_library()'s internal default value of ["//buildenv/target:gce"]
#     # because IREE targets are not compatible with `non_prod` constraint.
#     compatible_with = [],
#     deps = [
#         ":de_bufferization",
#         "@llvm-project//llvm:Support",
#         "@llvm-project//mlir:ArithDialect",
#         "@llvm-project//mlir:BufferizationDialect",
#         "@llvm-project//mlir:FuncDialect",
#         "@llvm-project//mlir:IR",
#         "@llvm-project//mlir:MemRefDialect",
#         "@llvm-project//mlir:Support",
#         "@llvm-project//mlir:TensorDialect",
#         "@llvm-project//mlir:Transforms",
#         "//tensorflow/compiler/xla/mlir_hlo:lhlo",
#         "//tensorflow/compiler/xla/service/gpu:gpu_executable",
#         "//tensorflow/compiler/xla/service/gpu:launch_dimensions",
#         "//tensorflow/compiler/xla/service/gpu:thunk",
#     ] + if_openxla(["//third_party/iree/llvm-external-projects/iree-dialects:IREEInputDialect"]),
# )
#
# cc_library(
#     name = "convert_memref_ops",
#     srcs = if_openxla(["convert_memref_ops.cc"]),
#     hdrs = if_openxla(["convert_memref_ops.h"]),
#     # TODO(ezhulenev): Override cc_library()'s internal default value of ["//buildenv/target:gce"]
#     # because IREE targets are not compatible with `non_prod` constraint.
#     compatible_with = [],
#     deps = [
#         ":de_bufferization",
#         "@llvm-project//mlir:ArithDialect",
#         "@llvm-project//mlir:FuncDialect",
#         "@llvm-project//mlir:IR",
#         "@llvm-project//mlir:MemRefDialect",
#         "@llvm-project//mlir:TensorDialect",
#         "@llvm-project//mlir:Transforms",
#     ] + if_openxla(["//third_party/iree/llvm-external-projects/iree-dialects:IREEInputDialect"]),
# )
#
# cc_library(
#     name = "convert_while_op",
#     srcs = if_openxla(["convert_while_op.cc"]),
#     hdrs = if_openxla(["convert_while_op.h"]),
#     # TODO(ezhulenev): Override cc_library()'s internal default value of ["//buildenv/target:gce"]
#     # because IREE targets are not compatible with `non_prod` constraint.
#     compatible_with = [],
#     deps = [
#         ":de_bufferization",
#         "@llvm-project//llvm:Support",
#         "@llvm-project//mlir:ArithDialect",
#         "@llvm-project//mlir:BufferizationDialect",
#         "@llvm-project//mlir:FuncDialect",
#         "@llvm-project//mlir:IR",
#         "@llvm-project//mlir:MemRefDialect",
#         "@llvm-project//mlir:SCFDialect",
#         "@llvm-project//mlir:TensorDialect",
#         "@llvm-project//mlir:Transforms",
#         "//tensorflow/compiler/xla/mlir_hlo:lhlo",
#     ] + if_openxla(["//third_party/iree/llvm-external-projects/iree-dialects:IREEInputDialect"]),
# )
#
# copybara:uncomment_end
