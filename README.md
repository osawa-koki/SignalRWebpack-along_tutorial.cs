# SignalRWebpack-along_tutorial.cs

マイクロソフト公式チュートリアルに沿って作成した、TypeScriptを使用したSignalRによるWebSocket通信を行う学習用プログラムです。

![サンプル画像](/dev/data/sample.gif)

## 対象のチュートリアル

- [TypeScript と Webpack を使用した ASP.NET Core SignalR の概要](https://learn.microsoft.com/ja-jp/aspnet/core/tutorials/signalr-typescript-webpack?view=aspnetcore-6.0&tabs=visual-studio)

## 実行方法

```shell
docker build -t signalr-chat-webpack .
docker run -p 80:7777 -it --rm --name my-signalr-chat-webpack signalr-chat-webpack

# 一行で書くなら、、、
docker build -t signalr-chat-webpack . && docker run -p 80:7777 -it --rm --name my-signalr-chat-webpack signalr-chat-webpack
```

## デプロイ設定(Render.com)

| キー | バリュー |
| ---- | ---- |
| Name | signalr-chat-webpack |
| Region | Oregon(US West) |
| Branch | main |
| Root Directory |  |
| Environment | Docker |
| Dockerfile Path | ./Dockerfile |
| Docker Build Context Directory |  |
| Docker Command |  |

## 開発環境

| 機能 | バージョン |
| ---- | ---- |
| Windows | 11 Home |
| Visual Studio | 2022 |
| .NET | 6.0 |
| C# | .NET依存 |
