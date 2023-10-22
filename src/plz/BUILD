go_library(
    name = "plz",
    srcs = ["plz.go"],
    pgo_file = "//:pgo",
    visibility = ["PUBLIC"],
    deps = [
        "///third_party/go/github.com_honeycombio_honeycomb-opentelemetry-go//:honeycomb-opentelemetry-go",
        "///third_party/go/github.com_honeycombio_otel-config-go//otelconfig",
        "///third_party/go/github.com_peterebden_go-cli-init_v5//flags",
        "///third_party/go/go.opentelemetry.io_otel//:otel",
        "//src/build",
        "//src/cli",
        "//src/cli/logging",
        "//src/core",
        "//src/fs",
        "//src/metrics",
        "//src/parse",
        "//src/remote",
        "//src/test",
    ],
)

go_test(
    name = "plz_test",
    srcs = ["plz_test.go"],
    deps = [
        ":plz",
        "///third_party/go/github.com_stretchr_testify//assert",
        "//src/cli",
        "//src/core",
    ],
)
