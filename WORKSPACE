load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "rules_python",
    url = "https://github.com/bazelbuild/rules_python/releases/download/0.1.0/rules_python-0.1.0.tar.gz",
    sha256 = "b6d46438523a3ec0f3cead544190ee13223a52f6a6765a29eae7b7cc24cc83a0",
)

# load("@rules_python//python:pip.bzl", "pip_repositories")
# pip_repositories()

# Only needed if using the packaging rules.
# load("@rules_python//python:pip.bzl", "pip_repositories")
# pip_repositories()


load("@rules_python//python:pip.bzl", "pip_install")

# # This rule translates the specified requirements.txt into
# # @my_deps//:requirements.bzl, which itself exposes a pip_install method.
# pip_import(
#    name = "3rdparty",
#    requirements = "//3rdparty/python:requirements.txt",
# )

# Load the pip_install symbol for my_deps, and create the dependencies'
# repositories.
pip_install(   # or pip_install
   name = "3rdparty",
   requirements = "//3rdparty/python:requirements.txt",
)


