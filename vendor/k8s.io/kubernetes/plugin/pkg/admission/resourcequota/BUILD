load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "admission.go",
        "config.go",
        "controller.go",
        "doc.go",
        "resource_access.go",
    ],
    importpath = "k8s.io/kubernetes/plugin/pkg/admission/resourcequota",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/hashicorp/golang-lru:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/meta:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apimachinery/announced:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apimachinery/registered:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/serializer:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/storage/etcd:go_default_library",
        "//vendor/k8s.io/client-go/util/workqueue:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/core:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/client/clientset_generated/internalclientset:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/client/informers/informers_generated/internalversion:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/client/listers/core/internalversion:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubeapiserver/admission:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/quota:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/quota/generic:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/util/reflector/prometheus:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/util/workqueue/prometheus:go_default_library",
        "//vendor/k8s.io/kubernetes/plugin/pkg/admission/resourcequota/apis/resourcequota:go_default_library",
        "//vendor/k8s.io/kubernetes/plugin/pkg/admission/resourcequota/apis/resourcequota/install:go_default_library",
        "//vendor/k8s.io/kubernetes/plugin/pkg/admission/resourcequota/apis/resourcequota/v1alpha1:go_default_library",
        "//vendor/k8s.io/kubernetes/plugin/pkg/admission/resourcequota/apis/resourcequota/validation:go_default_library",
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
        "//vendor/k8s.io/kubernetes/plugin/pkg/admission/resourcequota/apis/resourcequota:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
