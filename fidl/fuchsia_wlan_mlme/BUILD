# Copyright 2018 The Fuchsia Authors. All rights reserved.
# Use of this source code is governed by a BSD-style license that can be
# found in the LICENSE file.

# DO NOT MANUALLY EDIT!
# Generated by //scripts/sdk/bazel/generate.py.

licenses(["notice"])


load("//build_defs:fidl_library.bzl", "fidl_library")

package(default_visibility = ["//visibility:public"])

fidl_library(
    name = "fuchsia_wlan_mlme",
    library = "fuchsia.wlan.mlme",
    srcs = [
        "wlan_mlme.fidl",
        "wlan_mlme_ext.fidl",
    ],
    deps = [
        "//fidl/fuchsia_wlan_minstrel",
        "//fidl/fuchsia_wlan_stats",
    ],
)

load("//build_defs:cc_fidl_library.bzl", "cc_fidl_library")

cc_fidl_library(
    name = "fuchsia_wlan_mlme_cc",
    library = ":fuchsia_wlan_mlme",
    # TODO(DX-288): remove explicit deps once C++ compilation API is available
    #     in Skylark and generated through the cc_fidl_library rule.
    deps = [
        "//fidl/fuchsia_wlan_minstrel:fuchsia_wlan_minstrel_cc",
        "//fidl/fuchsia_wlan_stats:fuchsia_wlan_stats_cc",
    ],
)

load("//build_defs:dart_fidl_library.bzl", "dart_fidl_library")

dart_fidl_library(
    name = "fuchsia_wlan_mlme_dart",
    deps = [":fuchsia_wlan_mlme"],
)
