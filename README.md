# 代謝・内分泌 臨床計算・診療支援ツール

糖尿病・代謝・内分泌領域を中心に、臨床計算、病期・リスク分類、鑑別診断の補助、負荷試験判定、栄養管理などを1つのブラウザ画面で扱う医療従事者向けツールです。

## 公開URL

https://masao172.github.io/metano-endo-clinical-tools/

公開画面上部の著作権表示の下に「端末別利用マニュアル（PDF）」ボタンを設置しています。PDF表示は「× 閉じてツールに戻る」で閉じられます。

## 主な機能

- 糖代謝・インスリン分泌：HOMA、75gOGTT、グルカゴン負荷、低血糖鑑別など
- 電解質・酸塩基：血液ガス、低Na/高Na、低K/高K、高Caなど
- 内分泌：SIADH、甲状腺、下垂体・副腎負荷試験など
- 腎・栄養：CKD/糖尿病性腎症分類、肥満・糖尿病・CKDを考慮した栄養管理
- 脂質：LDL管理、Fredrickson/WHO表現型の参考推定、Friedewald LDL、non-HDL-C
- その他：FIB-4、TSAT、ABSI、インスリンポンプ初期設定など

## Webアプリ（PWA）として使う

この公開版はPWA対応です。GitHub PagesでHTTPS公開すると、ホーム画面へ追加して通常のアプリに近い形で起動できます。一度オンラインで読み込んだ後は、主要画面をオフラインでも起動できるようService Workerを組み込んでいます。

### iPhone / iPad

1. SafariでGitHub PagesのURLを開く
2. 共有ボタンをタップ
3. 「ホーム画面に追加」を選ぶ
4. 「追加」をタップ

### Android / Chrome

Chromeでサイトを開き、メニューの「アプリをインストール」または「ホーム画面に追加」を選びます。

> PWA機能は `file://` でHTMLを直接開いた場合には動作しません。GitHub PagesなどHTTPS上で使用してください。

## GitHub Pages

リポジトリ直下に、このフォルダ内のファイルをすべてアップロードしてください。`Settings` → `Pages` → `Deploy from a branch` → `main` / `/(root)` を選択します。

## データの扱い

入力値はブラウザ内のJavaScriptで処理されます。このHTMLには、入力値を外部へ送信する処理やブラウザ保存処理は組み込んでいません。

## 重要な注意

本ツールは医療従事者向けの判定補助ツールです。診断、処方、治療適応その他の医療判断を自動的に確定するものではありません。実際の診療では最新の添付文書、ガイドライン、検査法・測定系、施設基準および患者背景を確認してください。

## License

© 2026 大平征宏

Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)


## 同梱ファイル

- `manual.pdf`: 端末別利用マニュアル
- `qr-code.png`: 公開URLのQRコード
