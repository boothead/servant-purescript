package(default_visibility = ["//visibility:public"])

load(
  "@io_tweag_rules_haskell//haskell:haskell.bzl",
  "haskell_library",
  "haskell_binary",
  "haskell_toolchain",
)


haskell_binary(
  name = "server",
  main_file = "Main.hs",
  src_strip_prefix = "src",
  srcs = ["src/Counter/WebAPI.hs"],
  deps = ["//:servant-purescript"],
  prebuilt_dependencies = [
    "base"
  , "aeson"
  , "bytestring"
  , "containers"
  , "ghc-mod"
  , "http-api-data"
  , "http-types"
  , "lens"
  , "mainland-pretty"
  , "monad-logger"
  , "mtl"
  , "purescript-bridge"
  , "servant"
  , "servant-server"
  , "servant-subscriber"
  , "stm"
  , "text"
  , "transformers"
  , "wai"
  , "warp"

  ],
  visibility = ["//visibility:public"]
)

haskell_binary(
  name = "gen",
  main_file = "PSGenerator.hs",
  src_strip_prefix = "src",
  srcs = ["src/Counter/WebAPI.hs"],
  deps = ["//:servant-purescript"],
  prebuilt_dependencies = [
    "base"
  , "aeson"
  , "containers"
  , "filepath"
  , "ghc-mod"
  , "http-api-data"
  , "http-types"
  , "lens"
  , "mainland-pretty"
  , "purescript-bridge"
  , "servant"
  , "servant-foreign"
  , "servant-purescript"
  , "servant-subscriber"
  , "text"

  ],
  visibility = ["//visibility:public"]
)