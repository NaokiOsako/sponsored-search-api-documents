# ConversionTracker
ConversionTrackerオブジェクトは、コンバージョン測定タグやタグごとのパフォーマンスデータなどのコンバージョントラッカー情報を表します。

### Service
+ [ConversionTrackerService](../../services/ConversionTrackerService.md)

### Namespace
[ConversionTrackerService#Namespace](../../services/ConversionTrackerService.md#namespace)

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
 <tr>
  <td>conversionTrackerId</td>
  <td>xsd:long</td>
  <td>コンバージョントラッカーのIDです。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>Requirement</td>
  <td>-</td>
 </tr>
 <tr>
  <td>conversionTrackerName</td>
  <td>xsd:string</td>
  <td>コンバージョントラッカーの名称です。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Optional</br>Updatable</td>
  <td>-</td>
 </tr>
 <tr>
  <td>status</td>
  <td>enum <a href="ConversionTrackerStatus.md">ConversionTrackerStatus</a></td>
  <td>コンバージョントラッカーのステータスです。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>
 <tr>
  <td>category</td>
  <td>enum<br><a href="ConversionTrackerCategory.md">ConversionTrackerCategory</a></td>
  <td>トラッキング対象のコンバージョンのカテゴリです。<br>コンバージョン測定を行う目的をConversionTrackerCategoryより選んでください。<br>※電話コンバージョンの場合は、PAGE_VEIWの指定はできません。<br>※アプリコンバージョンの場合は、DEFAULTのみ指定可能です。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>
 <tr>
  <td>conversions</td>
  <td>xsd:long</td>
  <td>自動入札設定対象のコンバージョン数です。<br>ユニークコンバージョンか総コンバージョンかは、countingTypeに依存します。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>conversionValue</td>
  <td>xsd:string</td>
  <td>自動入札設定対象のコンバージョン値です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>allConversions</td>
  <td>xsd:long</td>
  <td>自動入札設定対象のコンバージョン数と、対象外のコンバージョン数の合計です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>allConversionVaule</td>
  <td>xsd:string</td>
  <td>自動入札設定対象のコンバージョン値と、対象外のコンバージョン値の合計です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>mostRecentConversionDate</td>
  <td>xsd:string</td>
  <td>直近のコンバージョン発生日です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>conversionTrackerType</td>
  <td>enum<br><a href="ConversionTrackerType.md">ConversionTrackerType</a></td>
  <td>コンバージョンタイプです。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Requirement</td>
  <td>-</td>
 </tr>
 <tr>
  <td>userRevenueValue</td>
  <td>xsd:string</td>
  <td>このコンバージョントラッカーに対するユーザー指定の収益値です。<br>1コンバージョンあたりの売上金額が固定値の場合、その金額を設定することで、売上金額をレポートなどで確認できます。<br>ADDリクエスト時に未指定の場合、0が設定されます。</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>
 <tr>
  <td>countingType</td>
  <td>enum<br><a href="ConversionCountingType.md">ConversionCountingType</td>
  <td>コンバージョンの計測方法です。<br>※Default：WebコンバージョンはMANY_PER_CLICK、<br>アプリコンバージョンはONE_PER_CLICK。</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional<br>default：MANY_PER_CLICK</td>
  <td>Optional</td>
  <td>-</td>
 </tr>
 <tr>
  <td>excludeFromBidding</td>
  <td>enum<br><a href="ExcludeFromBidding.md">ExcludeFromBidding</a></td>
  <td>自動入札設定で使用するかを表します。</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional<br>default: FALSE（使用する）</td>
  <td>Optional</td>
  <td>-</td>
 </tr>
 <tr>
  <td>measurermentPeriod</td>
  <td>xsd:int</td>
  <td>コンバージョン計測期間です（単位：日)。<br>7～90日間で設定可能です。<br>※アプリダウンロードの場合は30日間固定。</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional<br>default: 30</td>
  <td>Optional</td>
  <td>-</td>
 </tr>
</table>

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
