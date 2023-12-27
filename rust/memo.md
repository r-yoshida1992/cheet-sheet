# Rust commands

```sh 
# インストール関連
# install (MacOS)
curl --proto '=https' --tlsv1.3 https://sh.rustup.rs -sSf | sh
# C compiler install
xcode-select --install
# version confirm
rustc --version
# update
rustup update
# uninstall 
rustup self uninstall
# compile
rustc main.rs

# Cargo関連
# version confirm
cargo --version
# create project
cargo new project_name
# build(プロジェクトルートで実行する)
cargo build
# build and run(プロジェクトルートで実行する)
cargo run
# コンパイルするが実行ファイルを生成しない(コンパイル成功のみ確認)
cargo check
# リリースモジュールのビルド
cargo build --release
# 依存の更新
cargo update

# Tauri
# create app
cargo install create-tauri-app --locked
cargo create-tauri-app

# Tips
# マクロは呼び出す際に!がつく。
# CargoはRustにおけるビルドシステム及びパッケージマネージャー
# cargo new はvcsオプションをつけることでバージョン管理システムを指定したりすることができる
# cargo runはファイルが変更されていなければリビルドしない
# cargo buildした結果はtarget/debugに保存される(リリース用はtarget/release)
```
