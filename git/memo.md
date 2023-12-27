# Git Commands
```sh
# version確認
git version

# Gitリポジトリを作成する。(.gitディレクトリが作成され、カレントディレクトリがGit管理となる)
git init

# ファイルをステージングする
# ex: git add README.md
git add [file name]

# ステージングされているファイルをコミットする
git commit -m "commit message."

# Gitリポジトリ内の現在のブランチを変更する
# ex: git branch -M main
git branch -M [branch name]

# リモートリポジトリに関連づける
# ex: git remote add origin https://github.com/r-yoshida1992/cheet-sheet.git
git remote add origin [git url]

# コミットした変更をリモートリポジトリに反映する
# 初回は-u(--set-upstream)オプションをつけることで、ローカルブランチをリモートブランチに関連付けることができる
# 2回目以降はブランチ名を指定しないでもブランチに対する操作を行うことができる
git push -u origin main
git push --set-upstream origin main
# 2回目以降
git push

# リモートブランチの変更内容をローカルに反映する
git pull

# リモートブランチの情報をローカルに取得する
git fetch origin

# リモートのブランチをローカルにチェックアウト
# ex: git checkout -b main origin/main
git checkout -b [local branch name] [remote branch name]
# Git version 2.23以降
git switch -c [local branch name] [remote branch name]
```
