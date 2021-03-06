# StringData



crafttweakerのmod-idを持つmodによって追加されているクラスです。 従って、この機能を利用する場合はこのmodをインストールする必要があります。

## クラスのインポート
問題が発生した場合には、インポートが必要になります。とはいえ、お手数ですが予めインポートしておくほうが安全です。
```zenscript
crafttweaker.api.data.StringData
```

## 実装されたインターフェース
StringData は、以下のインターフェイスを実装しています。 つまり、利用可能な任意のメソッドはこのクラスでも使用できます。
- [crafttweaker.api.data.IData](/vanilla/api/data/IData)

## Constructors
```zenscript
new crafttweaker.api.data.StringData(Stringとして内部);
```
| パラメータ | タイプ  | 説明           |
| ----- | ---- | ------------ |
| 内部    | 文字列型 | 説明が提供されていません |



## メソッド
### asList

リストを取得<IData> この IData の表現は、 [crafttweaker.api.data.ListData](/vanilla/api/data/ListData) 以外の場合は null を返します。

 戻り値: `この IData がリストでない場合は null です。`

戻り値 List<[crafttweaker.api.data.IData](/vanilla/api/data/IData)>

```zenscript
new StringData("Hello").asList();
```

### asMap

この IData のマップ<String, IData> 表現を取得します。 [crafttweaker.api.data.MapData](/vanilla/api/data/MapData) 以外の場合は null を返します。

 戻り値: `この IData がマップでない場合は null です。`

戻り値 [crafttweaker.api.data.IData](/vanilla/api/data/IData)[String]

```zenscript
new StringData("Hello").asMap();
```

### asString

この IData の文字列表現を取得します

 戻り値: `この IData (値と型) を表す文字列。`

戻り値の文字列

```zenscript
new StringData("Hello").asString();
```

### を含む

Checks if this IData contains another IData, mainly used in subclasses of [crafttweaker.api.data.ICollectionData](/vanilla/api/data/ICollectionData), is the same as an equals check on other IData types

戻り値ブール値

```zenscript
new StringData("Hello").contains(data as crafttweaker.api.data.IData);
new StringData("Hello").contains("Display");
```

| パラメータ | タイプ                                                    | 説明                    |
| ----- | ------------------------------------------------------ | --------------------- |
| データ   | [crafttweaker.api.data.IData](/vanilla/api/data/IData) | それが含まれているかどうかを確認するデータ |


### コピー

このIDataのコピーを作成します。

 IData はデフォルトで変更不能です。これを使用してオブジェクトの適切なコピーを作成します。

 戻り値: `この IData のコピー`

戻り値 [crafttweaker.api.data.IData](/vanilla/api/data/IData)

```zenscript
new StringData("Hello").copy();
```

### getId

内部 NBT タグの ID を取得します。

 どの種類の NBT が格納されているかを決定するために使用されます(例えばリスト)

 戻り値: `このデータが表現する NBT タグの ID。`

バイトを返します

```zenscript
new StringData("Hello").getId();
```

### getString

内部 INBT タグの文字列表現を取得します。

 戻り値: `この IData の内部 INBT を表す文字列。`

戻り値の文字列

```zenscript
new StringData("Hello").getString();
```


## 演算子
### 追加

2 つの文字列 Datas を連結し、結果を返します。

```zenscript
new StringData("Hello") + data as crafttweaker.api.data.String Data
new StringData("Hello") + new StringData("World")
```

| パラメータ | タイプ                                                              | 説明        |
| ----- | ---------------------------------------------------------------- | --------- |
| データ   | [crafttweaker.api.data.StringData](/vanilla/api/data/StringData) | 追加する他のデータ |

