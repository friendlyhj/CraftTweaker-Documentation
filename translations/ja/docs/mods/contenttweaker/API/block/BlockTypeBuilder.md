# BlockTypeBuilder

特殊ブロック型の構築に使用される特殊ビルダーを示します。 [mods.contenttweaker.block.BlockTypeBuilder#withType](/mods/contenttweaker/API/block/BlockTypeBuilder/#withtype) で使用する

このクラスは mod-id `contenttweaker` を持つ mod によって追加されました。 従って、この機能を利用する場合はこのmodをインストールする必要があります。

## クラスのインポート
問題が発生した場合には、インポートが必要になります。とはいえ、お手数ですが予めインポートしておくほうが安全です。
```zenscript
mods.contenttweaker.block.BlockTypeBuilder
```

## 実装されたインターフェース
BlockTypeBuilder は、以下のインターフェースを実装します。 つまり、利用可能な任意のメソッドはこのクラスでも使用できます。
- [mods.contenttweaker.api.IIsBuilder](/mods/contenttweaker/API/api/IIsBuilder)

## メソッド
### ビルド

このビルダーが構築されると思われるものは何でも実際に構築するようCoTに指示します。

```zenscript
new BlockBuilder().withType<BlockBuilderBasic>().build(resourceLocation as String);
new BlockBuilder().withType<BlockBuilderBasic>().build("my_awesome_block");
```

| パラメータ   | タイプ  | 説明               |
| ------- | ---- | ---------------- |
| リソースの場所 | 文字列型 | このブロックを与えるリソースパス |



