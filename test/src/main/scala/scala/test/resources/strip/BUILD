load("//scala:scala.bzl", "scala_library","scala_specs2_junit_test")

scala_library(
   name = "noSrcsWithResources",
   resource_strip_prefix="test/src/main/scala/scala/test/resources/strip",
   resources  = ["nosrc_jar_resource.txt"]
)

scala_specs2_junit_test(
    name = "resouceStripPrefixTest",
    srcs = ["ResourceStripPrefixTest.scala"],
    deps = [":noSrcsWithResources"],
    size = "small",
    suffixes = ["Test"],
)
