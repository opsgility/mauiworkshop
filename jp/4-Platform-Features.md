## 演習 4: プラットフォーム機能へのアクセス

この演習では、.NET MAUI を使用して最も近いサルを見つけ、サルの位置を地図で開きます。

### インターネットの確認

.NET MAUI の組み込み `IConnectivity` を使用して、ユーザーがインターネットに接続しているかどうかを簡単に確認できます。

1. まず、.NET MAUI にある `IConnectivity` へのアクセスを取得しましょう。`IConnectivity` を `MonkeysViewModel` コンストラクターに注入します:

    ```csharp
    IConnectivity connectivity;
...