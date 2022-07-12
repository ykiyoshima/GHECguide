[前：GHEC Starter Guide](/GHEC_STARTER_GUIDE.md)　　　[次：GitHubのセットアップ](/GITHUB_SETUP.md)

# Gitのセットアップ

Gitとは、オープンソースのバージョン管理システムです。  
Gitを使うことで以下のようなことが可能となります。

- 最新のファイル + その前の古いファイルの一元管理
- ファイルのバージョンダウン（過去の内容に戻す）
- チーム開発におけるファイル編集履歴の共有や修正部分の統合

Gitをコンピューターにダウンロード・インストール・設定することで、コマンドラインでGitを使うことができます。

## Gitのセットアップ

### Windowsの場合
1. [https://git-scm.com/downloads](https://git-scm.com/downloads) にアクセスする  

1. Download for Windowsボタンをクリック  
    ![Gitダウンロードボタンの場所](/image/git_setup/git_download_page_220707.png)

1. Click here to download をクリック → Gitの.exeファイルダウンロードがスタート  
    ![Click here to downloadリンクの場所](/image/git_setup/git_download_link_220207.png)

1. ダウンロードした.exeファイルを開く  

1. すべてNextボタンをクリック → Installボタンが表示されたらInstallボタンをクリック

1. View Release Notesのチェックを外す → Finishボタンをクリック  
    ![Gitインストール完了ウィザード](/image/git_setup/complete_git_install_220207.png)

1. コンピューターを再起動する  

1. Git Bashを起動し、以下のコマンドを入力する  
`$ git config --global user.name "設定したいユーザー名"`

1. 以下のコマンドを入力してGitユーザー名が正しく設定されていることを確認する  
`$ git config --global user.name`

1. 以下のコマンドを入力する  
`$ git config --global user.email "設定したいメールアドレス"`

1. 以下のコマンドを入力してGitメールアドレスが正しく設定されていることを確認する  
`$ git config --global user.email`

### Macの場合
1. ターミナルにて以下のコマンドを入力する  
`$ brew -v`

1. `command not found: brew` と出力された場合は [https://brew.sh/index_ja](https://brew.sh/index_ja) にアクセスする（`Homebrew x.x.x` と出力された場合は2. ~ 7. をスキップする）

1. コマンド右隣のコピーアイコンをクリック  
    ![コマンドのコピーアイコンの場所](/image/git_setup/homebrew_220708.png)

1. ターミナルを開き、コピーしたコマンドを貼り付けてEnter  

1. `password:`と表示されたら、コンピューターにログインする際のパスワードを入力してEnter  

1. Enterを何回か押してインストールを実行（`Installation successful!` のような表示があればOK）  

1. 以下のコマンドを入力し、Homebrewがインストールされたことを確認  
`$ brew -v`

1. 以下のコマンドを入力する  
`$ brew install git`

1. 以下のコマンドを入力し、Gitがインストールされたことを確認  
`$ git version`

1. 以下のコマンドを入力する（何も出力されなければOK）  
`$ git config --global user.name "設定したいユーザー名"`

1. 以下のコマンドを入力してGitユーザー名が正しく設定されていることを確認する  
`$ git config --global user.name`

1. 以下のコマンドを入力する（何も出力されなければOK）  
`$ git config --global user.email "設定したいメールアドレス"`

1. 以下のコマンドを入力してGitメールアドレスが正しく設定されていることを確認する  
`$ git config --global user.email`

[前：GHEC Starter Guide](/GHEC_STARTER_GUIDE.md)　　　[次：GitHubのセットアップ](/GITHUB_SETUP.md)