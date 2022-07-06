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
    
## アカウントのセットアップ
OrganizationアカウントまたはEnterpriseアカウントのいずれかをセットアップします。<br><br>
**Organizationアカウント**  
複数人が様々なプロジェクトで共同作業を行うための共有アカウント  
オーナーと管理者は、データやプロジェクトへのアクセスを管理可能
<br><br>
**Enterpriseアカウント**  
複数のOrganizationアカウントを管理するためのアカウント  
オーナーは各Organizationアカウントのポリシー・課金・セキュリティを一元管理可能
<br><br>

### 【Organizationアカウントのセットアップ】
1. GitHubページ右上にあるプロフィール写真をクリック → Settingsをクリック
    ![Settingsの場所](/image/account1.png)

1. サイドバーのAccessセクションにあるOrganizationsをクリック
    ![Organizationの場所](/image/account2.png)

1. OrganizationsセクションにあるNew organizationボタンをクリック
    ![New_organizationボタンの場所](/image/account3.png)

1. Enterpriseプランを選択
    ![プラン比較ページ](/image/account4.png)

1. プロンプトにしたがってorganizationアカウントを作成

### 【Enterpriseアカウントのセットアップ】
1. GitHubページ右上にあるプロフィール写真をクリック → Settingsをクリック
    ![Settingsの場所](/image/account1.png)

1. サイドバーのAccessセクションにあるOrganizationsをクリック
    ![Organizationの場所](/image/account2.png)

1. 任意のOrganizationアカウント右隣のSettingsをクリック
    ![Organization_Settingsの場所](/image/account5.png)

1. サイドバーのAccessセクションにあるBilling and plansをクリック
    ![Organizationの場所](/image/account6.png)

1. 緑色のUpgrade to enterprise accountボタンをクリック
    ![Upgradeの場所](/image/account7.png)

1. Enterpriseプランを選択
    ![プラン比較ページ](/image/account8.png)

1. プロンプトにしたがってEnterpriseアカウントを作成

## GHECでのメンバーおよびチームの管理

### Organizationアカウントでのメンバーおよびチームの管理
Organizationアカウントにおける権限やメンバーのロール、チームの作成と管理、リポジトリへのアクセス権の付与が可能

1. GitHubページ右上にあるプロフィール写真をクリック → Your organizationsをクリック
    ![Your_organizationsの場所](/image/memberteams1.png)

1. 任意のOrganizationアカウント名のリンクをクリック
    ![Organizationアカウント名の場所](/image/memberteams2.png)

1. Organizationアカウント名の下にあるPeopleタグをクリック
    ![Peopleタグの場所](/image/memberteams3.png)

1. 緑色のInvite memberボタンをクリック
    ![Invite_memberボタンの場所](/image/memberteams4.png)

1. 招待したいメンバーのユーザーネーム or フルネーム or メールアドレスを入力 → 緑色のInviteボタンをクリック
    ![Inviteボタンの場所](/image/memberteams5.png)

1. 招待したいメンバーのロールを選択
    ![ロール選択ページ]()