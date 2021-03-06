# マンガでわかるGit ~ コマンド版 ~

[HOME](https://ginmarugh.github.io/memo/)

- [マンガでわかるGit ~ コマンド版 ~](https://www.r-staffing.co.jp/engineer/archive/category/%E3%83%9E%E3%83%B3%E3%82%AC%E3%83%BBGit)
  - [第1話 リポジトリの作成](https://www.r-staffing.co.jp/engineer/entry/20190621_1)
  - [第2話 ブランチの概念](https://www.r-staffing.co.jp/engineer/entry/20190719_1)
  - [第3話 マージの仕組み](https://www.r-staffing.co.jp/engineer/entry/20190830_1)
  - [第4話 コンフリクトの修正](https://www.r-staffing.co.jp/engineer/entry/20190927_1)
  - [第5話 git revert](https://www.r-staffing.co.jp/engineer/entry/20191025_1)
  - [第6話 git reset 3種類](https://www.r-staffing.co.jp/engineer/entry/20191129_1)
  - [第7話 git reflog](https://www.r-staffing.co.jp/engineer/entry/20191227_1)
  - [第8話 git switchとgit restore](https://www.r-staffing.co.jp/engineer/entry/20200131_1)
  - [第9話 git diff](https://www.r-staffing.co.jp/engineer/entry/20200228_1)
  - [第10話 git cherry-pick](https://www.r-staffing.co.jp/engineer/entry/20200327_1)
  - [第11話 git stash](https://www.r-staffing.co.jp/engineer/entry/20200424_1)
  - [第12話 git grep](https://www.r-staffing.co.jp/engineer/entry/20200605_1)
  - [第13話 git blame](https://www.r-staffing.co.jp/engineer/entry/20200626_1)
  - [第14話 git remote](https://www.r-staffing.co.jp/engineer/entry/20200717_1)
  - [第15話 .gitconfig](https://www.r-staffing.co.jp/engineer/entry/20200821_1)
  - [第16話 .gitconfigと.git/configで複数のGitアカウントと使い分ける](https://www.r-staffing.co.jp/engineer/entry/20200918_1)
  - [第17話 prune オプション](https://www.r-staffing.co.jp/engineer/entry/20201023_1)
  - [第18話 git tag](https://www.r-staffing.co.jp/engineer/entry/20201120_1)
  - [第19話 detached HEAD 状態って何？](https://www.r-staffing.co.jp/engineer/entry/20201225_1)

---

&nbsp;

- 01 リポジトリの作成
  - `git init`
  - `git status`
  - `git add <file-name>`
  - `git commit -m <commit-message>`
  - `git log`
- 02 ブランチの概念
  - `git branch <branch-name>`
  - `git switch <branch-name>`
  - `git checkout <branch-name>`
  - `git switch -c <branch-name>`
  - `git checkout -b <branch-name>`
- 03 マージの仕組み
  - `git merge <branch-name to be merged>`
- 04 コンフリクトの修正
  - `git commit -m <commit-message>`
  - `git merge --abort`
- 05 特定のコミットを打ち消す
  - `git revert <打ち消したいコミットID>`
- 06 特定の時点までファイルを巻き戻す
  - `git reset --soft <巻き戻したい時点のコミットを指定>`
  - `git reset --mixed <巻き戻したい時点のコミットを指定>`
  - `git reset --hard <巻き戻したい時点のコミットを指定>`
- 07 HEAD の移動履歴一覧を表示・特定の時点までファイルを巻き戻す
  - `git reflog`
  - `git reset --hard HEAD@{n}`
- 08 switchとrestore
  - `git switch <branch-name>`
  - `git restore <filename>`
- 09 差分を確認する
  - `git diff <変更前のコミット識別子>..<変更後のコミット識別子>`
- 10 特定のコミットの取り込み
  - `git cherry-pick <commit-ID>`
  - `git cherry-pick <commit-ID-1>..<commit-ID-2>`
  - `git cherry-pick -n <commit-ID>`
- 11 ファイルの一時退避
  - `git stash save`
  - `git stash list`
  - `git stash pop <stash-name>`
- 12 リポジトリ内を検索する
  - `git grep "検索したい文字列"`
  - `git grep "検索したい文字列" <コミット識別子>`
  - `git grep -l "検索したい文字列"`
- 13 コミットした人の名前と日時を表示する
  - `git blame <file-name>`
- 14 リモートリポジトリの追加・削除
  - `git remote add <remote-repository-name> <remote-repository-url>`
  - `git remote rm <remote-repository-name>`
  - `git remote -v`
- 15 .gitconfigファイルの編集
  - `git config --global --edit`
- 16 リポジトリごとにユーザー名、ユーザーメイルアドレスを使い分ける
  - `git config --global user.name "wakaba"`
  - `git config --global user.email. "wakaba@example.com"`
  - `git config user.name "wakaba2"`
  - `git config user.email "wakaba2@example.com"`
- 17 リモート追跡ブランチの削除
  - `git fetch --prune`
  - `git remote prune <remote-repository-name>`
- 18 タグを付ける
  - `git tag <tag-name>`
  - `git push origin <tag-name>`
- 19 detached HEADを解決する
  - `git branch <branch-name>`

&nbsp;
