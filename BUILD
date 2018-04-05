package(default_visibility = ["//visibility:public"])

load(
  "@io_tweag_rules_haskell//haskell:haskell.bzl",
  "haskell_library",
  "haskell_toolchain",
)

haskell_toolchain(
  name = "ghc",
  version = "8.2.2",
  tools = "@ghc//:bin",
)

haskell_library(
  name = "servant-purescript",
  src_strip_prefix = "src",
  srcs = glob(['src/**/*.hs']),
  prebuilt_dependencies = [
    "base"
  , "aeson"
  , "bytestring"
  , "containers"
  , "directory"
  , "filepath"
  , "http-types"
  , "lens"
  , "mainland-pretty"
  , "purescript-bridge"
  , "servant"
  , "servant-foreign"
  , "servant-server"
  , "servant-subscriber"
  , "text"
  ],
)
