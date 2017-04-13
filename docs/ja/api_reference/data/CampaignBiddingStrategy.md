# CampaignBiddingStrategy
CampaignBiddingStrategyオブジェクトは、自動入札設定方法を表します。<br>

### Service
+ [CampaignService](../services/CampaignService.md)

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
  <td>biddingStrategyId</td>
  <td>xsd:long</td>
  <td> 自動入札IDです。</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional</td>
  <td>Optional<br><i>Updatable</i></td>
  <td>-</td>
 </tr>
 <tr>
  <td>biddingStrategyName</td>
  <td>xsd:string</td>
  <td>自動入札名です。<br>※50文字以内になります。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>biddingStrategyType</td>
  <td>enum <a href="./BiddingStrategyType.md">BiddingStrategyType</a></td>
  <td>自動入札タイプです。</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional</td>
  <td>Optional<br><i>Updatable</i></td>
  <td>-</td>
 </tr>
 <tr>
  <td>biddingStrategySource</td>
  <td>enum <a href="./BiddingStrategySource.md">BiddingStrategySource</a></td>
  <td>入札ソースです。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>biddingScheme</td>
  <td><a href="./BiddingScheme_nonBiddingStrategy.md">BiddingScheme</a><br> inherited <a href="./ManualCpcBiddingScheme.md">ManualCpcBiddingScheme</a><br> inherited <a href="./BudgetOptimizerBiddingScheme.md">BudgetOptimizerBiddingScheme </a><br> inherited <a href="./EnhancedCpcBiddingScheme_nonBiddingStrategy.md">EnhancedCpcBiddingScheme</a><br> inherited <a href="./PageOnePromotedBiddingScheme_nonBiddingStrategy.md">PageOnePromotedBiddingScheme </a><br> inherited <a href="./TargetCpaBiddingScheme_nonBiddingStrategy.md">TargetCpaBiddingScheme</a><br> inherited <a href="./TargetSpendBiddingScheme_nonBiddingStrategy.md">TargetSpendBiddingScheme</a><br> inherited <a href="./TargetRoasBiddingScheme_nonBiddingStrategy.md">TargetRoasBiddingScheme</a></td>
  <td>自動入札設定の詳細です。<br>※BudgetOptimizerBiddingSchemeは現在設定できません。同項目を設定していたキャンペーンには、2017年4月12日にTargetSpendBiddingSchemeが設定されました。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
</table>

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
