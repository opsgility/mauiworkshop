## 演習 5: CollectionView の探索

### タスク 1: 自動更新の有効化

.NET MAUI の `ListView` にはプル・トゥ・リフレッシュのサポートが組み込まれていますが、`RefreshView` を使用すると、`ScrollView` や `CollectionView` などの他のコントロールにもプル・トゥ・リフレッシュを追加できます。

`RefreshView` を追加して、`CollectionView` にプル・トゥ・リフレッシュ機能を追加しましょう。

`CollectionView` ロジックを以下のように `RefreshView` でラップして更新します:

```xml
<CollectionView
    Grid.ColumnSpan="2"
    ItemsSource="{Binding...