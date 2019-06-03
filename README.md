# Swift_TCPSocket

チャットサーバーの作成方法
1. ディレクトリを作成して移動
2.  "swift package init"を実行
3. Package.swift の dependencies に swift-nio のリポジトリを追加
import PackageDescription

let package = Package(
name: "ChatServer",

...    

dependencies: [
.package(url: "https://github.com/apple/swift-nio.git", from: "1.0.0")
],

...
)

4.ビルドしてChatサーバーを起動

❯ swift build

// 起動するとデフォルトポートは 9999 になります
❯ swift run NIOChatServer
