java_library(
    name = "hadoop",
    srcs = glob([
        "hadoop/src/main/java/org/tensorflow/hadoop/io/*.java",
        "hadoop/src/main/java/org/tensorflow/hadoop/util/*.java",
    ]),
    deps = [
        "//maven/jetty9-hadoop1/org.apache.hadoop/hadoop-common",
        "//maven/jetty9-hadoop1/org.apache.hadoop/hadoop-mapreduce-client-core"
    ],
    visibility = ["//visibility:public"],
)
