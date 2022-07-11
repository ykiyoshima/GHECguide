[前：リポジトリの操作](/REPOSITORY.md)　　　[次：OrganizationアカウントまたはEnterpriseアカウントのセットアップ](/ACCOUNT.md)

# チーム開発におけるリポジトリの操作

複数人で共通のソースコードを管理する際に便利な機能がGitには備わっています。  
特にブランチという仕組みを活用することで、あるバージョンはリリース用として公開しつつ、ブランチを使って開発用の別バージョンも並行して管理する、といったことが可能になります。

## リポジトリのクローン

クローン：既存のリモートリポジトリからソースコードを複製すること  
 
1. GitHub上でクローンしたいリモートリポジトリを開く → 緑色のcodeボタンをクリック → HTTPSが選択されていることを確認 → コピーアイコンをクリック  
    ![リポジトリURLの場所](/image/team_repository/repository_url_220708.png)

1. コマンドライン上で、クローンしたソースコードの保存先にしたいディレクトリへ移動  

1. 以下のコマンドを入力（「https://」以降はコピーしたURLを貼り付ければOK）  
`$ git clone https://github.com/xxx/xxx.git`

1. クローンが完了

## ブランチの作成および操作

ブランチ：同時進行で開発を行うためにソースコードを枝分かれさせること

1. 以下のコマンドを入力（例：featureブランチを新たに作成）  
`$ git branch feature`

1. 作業ブランチを変更したい場合は以下のコマンドを入力  
`$ git checkout feature`

1. 以下のコマンドを入力 → ローカルリポジトリにあるブランチ一覧を表示（「*」は現在作業中のブランチを示す）  
    ```
    $ git branch
    * feature
      main
    ```

1. 新しく作成したブランチでの作業をリモートリポジトリに反映させたい場合は以下の流れでコマンドを実行  
`$ git add .`  
`$ git commit -m "コミットメッセージ"`  
`$ git push origin feature`

## マージとプルリクエスト

マージ：あるブランチの変更内容を別のブランチにも反映させること   
プルリクエスト：マージしてよいかどうか他のメンバーへ確認を依頼すること  

### プルリクエストの作成

1. GitHub上の作業中リモートリポジトリのトップページに遷移 → 緑色のCompare & pull requestボタンをクリック  
    ![Compare_&_pull_requestボタンの場所](/image/team_repository/start_pull_request_220711.png)

1. マージ先、マージ元を選択 → タイトル、コメントを入力 → 緑色のCreate pull requestボタンをクリック  
    ![Pull_request画面](/image/team_repository/pull_request_220711.png)

1. プルリクエスト作成が完了  

### プルリクエストの修正依頼

プルリクエストの内容に問題がある場合、以下の手順でプルリクエスト申請者に修正依頼を行います。  

1. Pull requestsタブをクリック → Files changedタブをクリック → 修正を依頼したい箇所にカーソルを合わせ、青い＋ボタンをクリック → レビューコメントを記入 → 緑色のStart a reviewボタンをクリック  
    ![Files_changed画面](/image/team_repository/files_changed_220711.png)

1. 緑色のReview changesボタンをクリック → 緑色のSubmit reviewボタンをクリック
    ![Submit_reviewボタンの場所](/image/team_repository/submit_review_220711.png)

1. 修正依頼が完了

### プルリクエストの承認（マージ）

プルリクエストの内容に問題がない場合、以下の手順でプルリクエストの内容をマージします。  

1. Pull requestsタブをクリック → Conversationタブをクリック → 緑色のMerge pull requestボタンをクリック → 緑色のConfirm mergeボタンをクリック  
    ![Conversation画面](/image/team_repository/conversation_220711.png)

1. 緑色のConfirm mergeボタンをクリック
    ![Confirm_mergeボタンの場所](/image/team_repository/confirm_merge_220711.png)

1. マージが完了

## リモートリポジトリからローカルリポジトリへのプル

プル：マージにより更新されたリモートリポジトリをローカルリポジトリに反映させること

1. 以下のコマンドを入力し、作業ブランチをプル先にしたいブランチ（例：ローカルリポジトリのmain）に変更する  
`$ git checkout main`

1. 以下のコマンドを入力し、プル元（例：リモートリポジトリのmain）のブランチからプル先へ変更内容を反映させる  
`$ git pull origin main`

1. プルが完了

[前：リポジトリの操作](/REPOSITORY.md)　　　[次：OrganizationアカウントまたはEnterpriseアカウントのセットアップ](/ACCOUNT.md)