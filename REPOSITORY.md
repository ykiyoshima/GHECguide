[前：GitHubのセットアップ](/GITHUB_SETUP.md)　　　[次：OrganizationアカウントまたはEnterpriseアカウントのセットアップ](/ACCOUNT.md)

# リポジトリの操作

リモートリポジトリはGitHub上から、ローカルリポジトリは作業ディレクトリ上にてコマンドラインツールを使用してそれぞれ作成できます。

## リモートリポジトリの作成

1. [https://github.com/](https://github.com/) にアクセスし、サインインする  

1. 緑色のCreate repositoryボタンをクリック
    ![Create_repositoryボタンの場所](/image/github_create_repository_220708.png)

1. 任意のリポジトリ名を入力 → Public（誰でも閲覧可能） or Private（閲覧者を制限）を選択 → 緑色のCreate repositoryボタンをクリック
    ![Create_a_new_repositoryページ](/image/create_a_new_repository_220708.png)

1. リモートリポジトリの作成が完了

## ローカルリポジトリの作成

1. 任意のディレクトリを作成

1. コマンドラインツールを起動し、作成したディレクトリに移動

1. 目的のディレクトリに移動したことを確認 → 以下のコマンドを入力  
`$ git init`

1. ローカルリポジトリの作成が完了

## ローカルリポジトリへのコミット
コミット：ファイルの追加や変更をローカルリポジトリに反映する操作

1. 任意のファイルを作成（例：index.html）  

1. 以下のコマンドを入力（末尾の「.」を忘れないように注意）  
`$ git add .`

1. 以下のコマンドを入力（コミットメッセージは""で囲む）  
`$ git commit -m "任意のコミットメッセージ"`

1. ローカルリポジトリへのコミットが完了

## リモートリポジトリへのプッシュ
プッシュ：ローカルリポジトリへの変更をリモートリポジトリに反映する操作

1. GitHubの右上にあるアイコンをクリック → Your repositoriesをクリック  
    ![Your_repositoriesの場所](/image/from_icon_to_your_repositories_220708.png)

1. プッシュ先にしたいリモートリポジトリ名をクリック  
    ![リモートリポジトリ名の場所](/image/your_repositories_220708.png)

1. HTTPSが選択されていることを確認 → コピーアイコンをクリック  
    ![リモートリポジトリのコード](/image/remote_repository_code_220708.png)

1. 以下のコマンドを入力（「https://」から始まる文字列は先ほどコピーしたものを直接貼り付ければOK）  
`$ git remote add origin https://github.com/xxx/xxx.git`

1. 以下のコマンドを入力  
`$git push origin main`

1. リモートリポジトリへのプッシュが完了

[前：GitHubのセットアップ](/GITHUB_SETUP.md)　　　[次：OrganizationアカウントまたはEnterpriseアカウントのセットアップ](/ACCOUNT.md)