
add //セーブしたい内容を追加
add. //変更した全てのファイルを追加する

commit // セーブポイント
commit -m "コメント" //コメント

push // アップロード

---
### パソコンの流れ
1. フォルダを作る
2. gitのローカルリポジトリ（貯蔵庫）をつくる
git init（初期化）
3. コードを書く
4. add
5. commit
---

■コマンド
pwd // 今開いているフォルダの場所を確認

---
git config --global user.name 'xxx'
git config --global user.email 'xxx'

git config --list //Qで抜けれる

---

### 2回目以降は3つのコマンド
git add .
// VSCode上で追加ファイルも見れる

git commit -m "コメント"
// VScode上GitGraphでIDも見れる

git push origin main
// リモート名 リモートブランチ

---

git push -u 付け忘れた時

最初にリモートリポジトリにアップする時に「-u」を付け忘れると、
毎回アップの際は「git push origin main」とつける必要がある。
これをブランチ名を指定することで、「git push」のみでアップできるようになる。

上流ブランチの変更
git branch -u リモートリポジトリ名/ブランチ名
「git branch -u origin/main」

上流ブランチの設定確認
git branch -vv

---

GitHubにアップしたくないファイル・フォルダを書いておく

.gitignore


---

### git branch（ブランチ）

* ブランチの確認
git branch
* ブランチの作成
git branch \<new>
* ブランチ名変更
git branch -m \<old> \<new>
* ブランチの切替
git switch "ブランチ名"
* 新ブランチ作成＋切替
git switch -c \<new>
* ブランチの削除
git branch -d <ブランチ名>

補足
昔は checkout でブランチの切替を行っていた。
