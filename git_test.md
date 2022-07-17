
add //セーブしたい内容を追加
add. //変更した全てのファイルを追加する

commit // セーブポイント
commit -m "コメント" //コメント

push // アップロード

----------------------------------
### パソコンの流れ
1. フォルダを作る
2. gitのローカルリポジトリ（貯蔵庫）をつくる
git init（初期化）
3. コードを書く
4. add
5. commit
----------------------------------

■コマンド
pwd // 今開いているフォルダの場所を確認

----------------------------------
git config --global user.name 'xxx'
git config --global user.email 'xxx'

git config --list //Qで抜けれる
----------------------------------

### 2回目以降は3つのコマンド
git add .
// VSCode上で追加ファイルも見れる

git commit -m "コメント"
// VScode上GitGraphでIDも見れる

git push origin main
// リモート名 リモートブランチ


