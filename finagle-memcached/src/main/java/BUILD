java_library(
    sources = ["**/*.java"],
    compiler_option_sets = {"fatal_warnings"},
    provides = artifact(
        org = "com.twitter",
        name = "finagle-memcached-java",
        repo = artifactory,
    ),
    dependencies = [
        "3rdparty/jvm/com/google/guava",
        "3rdparty/jvm/com/google/inject:guice",
        "3rdparty/jvm/org/scala-lang:scala-library",
        "finagle/finagle-core/src/main/scala",
        "finagle/finagle-memcached/src/main/scala",
        "util/util-core/src/main/scala",
        "util/util-function/src/main/java",
        "util/util-stats/src/main/scala",
    ],
)

# TODO: Remove this and references to it,
# when a fix for https://github.com/pantsbuild/pants/issues/7200 has landed.
files(
    name = "pants-workaround",
    sources = ["**/*.java"],
)
