load("@build_stack_rules_hugo//hugo:rules.bzl", "hugo_site", "hugo_theme")

hugo_theme(
    name = "book",
    srcs = [
        "@com_github_alex_shpak_hugo_book//:files",
    ],
)

hugo_site(
    name = "site",
    config = "config.yaml",
    content = glob(["content/**"]),
    theme = ":book",
)
