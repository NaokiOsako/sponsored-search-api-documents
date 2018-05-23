# AccountOperation
AccountOperation object describes account information for operation of mutate method and list of operations.
### Service
+ [AccountService](../../services/AccountService.md)
### Namespace
[AccountService#Namespace](../../services/AccountService.md#namespace)

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
  <td colspan="8">Operation(inherited)</td>
 </tr>
 <tr>
  <td>operator</td>
  <td>enum <br>
  Operator</td>
  <td>Available to use:SET</td>
  <td colspan="5"></td>
 </tr>
 <tr>
  <td colspan="8">AccountOperation</td>
 </tr>
 <tr>
  <td>accountId</td>
  <td>xsd:long</td>
  <td>Account ID.</td>
  <td>-</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Requirement</td>
  <td>Requirement</td>
 </tr>
 <tr>
  <td>operand[]</td>
  <td><a href="Account.md">Account</a></td>
  <td>Array of Account object. Each array involves account information for operation.</td>
  <td>-</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Requirement</td>
  <td>Requirement</td>
 </tr>
</table>

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
