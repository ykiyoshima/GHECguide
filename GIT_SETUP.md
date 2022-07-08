[前：GHEC Starter Guide](/GHEC_STARTER_GUIDE.md)　　　[次：GitHubのセットアップ](/GITHUB_SETUP.md)

# Gitのセットアップ

Gitとは、オープンソースのバージョン管理システムです。  
Gitを使うことで以下のようなことが可能となります。

- 最新のファイル + その前の古いファイルの一元管理
- ファイルのバージョンダウン（過去の内容に戻す）
- チーム開発におけるファイル編集履歴の共有や修正部分の統合

Gitをコンピューターにダウンロード・インストール・設定することで、コマンドラインでGitを使うことができます。

## Gitのセットアップ
1. [https://git-scm.com/downloads](https://git-scm.com/downloads) にアクセスする  

1. Download for 〇〇ボタンをクリック  
    ![Gitダウンロードボタンの場所](/image/git_download_page_220707.png)

1. Click here to download をクリック → Gitの.exeファイルダウンロードがスタート  
    ![Click here to downloadリンクの場所](/image/git_download_link_220207.png)

1. ダウンロードした.exeファイルを開く  

1. すべてNextボタンをクリック → Installボタンが表示されたらInstallボタンをクリック

1. View Release Notesのチェックを外す → Finishボタンをクリック  
    ![Gitインストール完了ウィザード](/image/complete_git_install_220207.png)

1. コンピューターを再起動する  

1. Windowsの場合はGit Bash、Macの場合はターミナルにて（以下Gitコマンドは同じツールから行う）以下のコマンドを入力する  
`$ git config --global user.name "設定したいユーザー名"`

1. 以下のコマンドを入力してGitユーザー名が正しく設定されていることを確認する  
`$ git config --global user.name`

1. 以下のコマンドを入力する  
`$ git config --global user.email "設定したいメールアドレス"`

1. 以下のコマンドを入力してGitメールアドレスが正しく設定されていることを確認する  
`$ git config --global user.email`

[前：GHEC Starter Guide](/GHEC_STARTER_GUIDE.md)　　　[次：GitHubのセットアップ](/GITHUB_SETUP.md)