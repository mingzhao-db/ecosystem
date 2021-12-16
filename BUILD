load("//bazel/rules:cross_scala_lib.bzl", "cross_scala_lib", "DEFAULT_CROSS_TREE", "SPARK_3_0_CROSS_TREE")
load("//spark/versions:cross_build_utils.bzl", "SPARK_3_0_ALL_MAVEN_DEPS", "SPARK_3_0_MAVEN_TREE", "SPARK_3_1_ALL_MAVEN_DEPS", "SPARK_3_1_MAVEN_TREE", "SPARK_3_2_ALL_MAVEN_DEPS", "SPARK_3_2_MAVEN_TREE", "SPARK_3_3_ALL_MAVEN_DEPS", "SPARK_3_3_MAVEN_TREE")
load("//spark/versions:spark.bzl", "SPARK_VERSIONS")

cross_scala_lib(
    base_name = "hadoop",
    emit_ijar = False,
    srcs = glob([
        "hadoop/src/main/java/org/tensorflow/hadoop/io/*.java",
        "hadoop/src/main/java/org/tensorflow/hadoop/util/*.java",
    ]),
    cross_trees = [SPARK_3_0_CROSS_TREE],
    cross_scala_versions = ["2.11", "2.12"],
    cross_deps = [
    ],
    deps = [
        "{parent}/org.apache.hadoop/hadoop-common",
        "{parent}/org.apache.hadoop/hadoop-mapreduce-client-core",
    ],
    cross_exports = [
    ],
    visibility = ["//visibility:public"],
)

