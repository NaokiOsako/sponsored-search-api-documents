# AccountPage
AccountPageオブジェクトは、取得されるアカウントに関するエントリーを表します。

### Service
+ [AccountService](../../services/AccountService.md)

### Namespace
[AccountService#Namespace](../../services/AccountService.md#namespace)

| フィールド | データ型 | 説明 |
|---|---|---|
| Page(inherited)|||
| totalNumEntries| xsd:int| 取得される項目の総件数です。 |
| Page.Type| xsd:string| このインスタンスのPageのサブタイプです。 |
| AccountPage|||
| values[]| <a href="AccountValues.md">AccountValues</a>| AccountValuesオブジェクトの配列です。各配列には、操作結果およびアカウント情報が含まれます。 |

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
