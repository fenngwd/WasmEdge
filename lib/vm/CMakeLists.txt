# SPDX-License-Identifier: Apache-2.0

wasmedge_add_library(wasmedgeVM
  vm.cpp
)

target_link_libraries(wasmedgeVM
  PUBLIC
  wasmedgeCommon
  wasmedgeAST
  wasmedgeLoader
  wasmedgeValidator
  wasmedgeInterpreter
  wasmedgeHostModuleWasi
  wasmedgeHostModuleWasmEdgeProcess
)
