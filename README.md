# swiftlint_on_pre_push
リモートリポジトリにpushする前にSwiftLintのチェックを行うサンプルプロジェクト


```/bin/sh
# SwiftLintをインストール（Homebrewを使う想定）
$ brew install swiftlint

# プロジェクトをclone
$ git clone git@github.com:zrn-ns/swiftlint_on_pre_push.git
$ cd swiftlint_on_pre_push

# githooksのパスを変更
$ git config --local core.hooksPath .githooks/

# Remoteブランチの向き先を変更
$ git remote set-url origin {new url}

# pushする（Lintチェックが行われる）
$ git push origin HEAD
```
