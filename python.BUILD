# Description:
#   Build rule for Python and Numpy.
#   This rule works for Debian and Ubuntu. Other platforms might keep the
#   headers in different places, cf. 'How to build DeepMind Lab' in build.md.

cc_library(
    name = "python",
    hdrs = glob([
        "3.6.3/include/python3.6m/*.h",
        "3.6.3/lib/python3.6/site-packages/numpy/core/include/numpy/*.h",
    ]),
    includes = [
        "3.6.3/include/python3.6m",
        "3.6.3/lib/python3.6/site-packages/numpy/core/include",
    ],
    visibility = ["//visibility:public"],
)
