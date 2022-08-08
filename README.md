# クラウドプラットフォーム実習 Ⅰ

## 第 2 回 課題レポート

### テーマ

ボルトアクションエアーライフルの命中判定を、ターゲットに BB 弾が着弾した音から機械学習により判別し、Slack API を通じてデバイスに通知を得る。

### 使い方

0. 必要なもの

- Slack
- Chrome 等のブラウザ

1. リポジトリをクローンします

```shell
$ git clone https://github.com/Taipoon/cpp2-l96-judgeAI.git
```

2. Slack API のエンドポイント URL を作成します
   こちらの記事を参考にして Webhook の URL を取得してください。

   > https://qiita.com/cawpea/items/98e6271f627c3b9a5e12

3. Slack Webhook URL を設定します

index.html の 76 行目あたりにある以下のコードを探し、

```javascript
// Slack Webhook URL
const SLACK_URL = "YOUR SLACK URL HERE";
```

`YOUR SLACK URL HERE`の部分に[2]で取得した Slack Webhook URL を入力します。

3. index.html をブラウザで開きます
   ブラウザにカメラまたはマイクの使用権限を許可します。
