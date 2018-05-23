# FeedItemReturnValue
FeedItemReturnオブジェクトは、フィードアイテムの情報を格納します。

### Service
+ [FeedItemService](../../services/FeedItemService.md)

### Namespace
[FeedItemService#Namespace](../../services/FeedItemService.md#namespace)

<table>
 <tr>
  <th>Field</th>
  <th>Type</th>
  <th>Description</th>
  <th>response</th>
  <th>get</th>
  <th>add</th>
  <th>set</th>
  <th>remove</th>
 </tr>
 <tr>
  <td colspan="8"><a href="../Common/ListReturnValue.md">ListReturnValue</a>(inherited)</td>
 </tr>
 <tr>
  <td>ListReturnValue.Type</td>
  <td>xsd:string</td>
  <td>このインスタンスの ListReturnValue のサブタイプを示します。</td>
  <td colspan="5"></td>
 </tr>
 <tr>
  <td>Operation.Type</td>
  <td>xsd:string</td>
  <td>mutate処理の内容です。 </td>
  <td colspan="5"></td>
 </tr>
 <tr>
  <td colspan="8">FeedItemReturnValue</td>
 </tr>
 <tr>
  <td>values[0...2000]</td>
  <td><a href="FeedItemValues.md">FeedItemValues</a></td>
  <td>フィードアイテムに関する 情報です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
</table>

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
