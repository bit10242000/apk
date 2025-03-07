package(
    default_visibility = ["//src:__subpackages__"],
)
load("@rules_kotlin//kotlin:kotlin.bzl", "kt_android_library")
load("@rules_kotlin//kotlin:kotlin.bzl", "kt_jvm_library")

kt_jvm_library(
    name = "le_activity_kt",
    srcs = glob(["ladiesempire/**/*.kt"], allow_empty=True),
    deps = [
        "@rules_android//android:android_sdk",
    ]
)
kt_android_library(
    name = "le_activity",
    srcs = [
        "MainActivity.kt",
    ],
    manifest = "Manifests/AndroidManifest.xml",
    resource_files = glob(["res/**"], allow_empty=True),
    deps = [
        ":le_activity_kt",
        "@rules_android//android:android_sdk",
    ],
)