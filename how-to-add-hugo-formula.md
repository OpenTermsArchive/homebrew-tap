# How to create a Hugo formula

1. Copy and paste the latest version of forumla de Hugo available.
2. Replace the version number in the filename: `hugo@<version>.rb`
3. Copy and paste the formula published in the [homebrew-core respoitory](https://github.com/Homebrew/homebrew-core/commits/master/Formula/h/hugo.rb) that corresponds to the desired version of Hugo you want. For example `https://github.com/Homebrew/homebrew-core/blob/969c13371ba1e5a593ee4de2194310ec76ef2535/Formula/h/hugo.rb`
4. Edit the classname with the following format: `<hugo>AT<version>. Exemple, for the version '0.146.0` the classname is `HugoAT01464`.
5. Delete the code section of `bottle do`
6. Replace `system "go", "build", *std_go_args(ldflags:, tags:)` by `system "go", "build", *std_go_args(ldflags:, tags:, output: bin/"hugo")`
7. Commit and push.
