licenses(["notice"])  # Apache 2.0

package(default_visibility = ["//visibility:public"])

py_library(
    name = "metrics",
    srcs = [
        "__init__.py",
        "cohens_kappa.py",
        "f_scores.py",
        "hamming.py",
        "matthews_correlation_coefficient.py",
        "multilabel_confusion_matrix.py",
        "r_square.py",
        "utils.py",
    ],
    deps = [
        "//tensorflow_addons/testing",
        "//tensorflow_addons/utils",
    ],
)

py_test(
    name = "metrics_test",
    size = "small",
    srcs = glob(["*_test.py"]),
    main = "run_all_test.py",
    deps = [
        ":metrics",
    ],
)
