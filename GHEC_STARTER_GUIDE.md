[次：GHEC Starter Guide](/GHEC_STARTER_GUIDE.md)
<br><br>

# GitHub Enterprise Cloud Starter Guide
本資料はGitHub Enterprise Cloud（以下、GHEC）の概要および導入の手引きを記載したものです。
本資料はGHECのアップデートによって適宜修正されます。
また本資料はGitHub公式ドキュメントをもとに構成しています。

[Getting started with GitHub Enterprise Cloud](https://docs.github.com/ja/get-started/onboarding/getting-started-with-github-enterprise-cloud)

## GitHub Enterprise Cloudとは
GHECはGitHubをエンタープライズレベルで利用するための機能が一通り提供されています。
- 無制限のパブリック/プライベートリポジトリ
- 無制限のコラボレータ
- GitHub Actions 50,000分/月
- GitHub Packagesストレージ 総計50GB
- コミュニティボードによるサポート
- 必須レビューワー
- コードオーナー
- SAMLシングル・サインオン
- 高度な監査機能

[GitHub Enterprise 公式サイト](https://github.co.jp/enterprise.html)

## ライセンス形態
GHECのライセンスは通常GitHubアカウントに付与されます。
- GHECライセンスは1つのGitHubアカウントに1つ付与することができます。
- GHECライセンスを付与したGitHubアカウントを弊社から払い出しません。
- GHECライセンスはEnterprise管理者からGitHubアカウントに付与することが可能です。

### GHECライセンスのカウント
GHECライセンスはGitHub内のEnterpriseに紐づく全てのGitHubアカウントに付与します。

flowchart LR
    id3(View) -- User actions --> id2 -- Update UI --> id3(View)
<br><br>
[次：アカウントのセットアップ](/ACCOUNT.md)