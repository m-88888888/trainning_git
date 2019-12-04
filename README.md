# gitとgithubの勉強

## 直前のコミットの上書き
```
git commit --amend
```
viで直前のコミットを修正できて、メッセージを修正したり、ファイルを追加したら
:wqコマンドで上書き保存する。
次のようなログが出る。
```
m-88888888:trainning_git hachi$ git commit -m "test message"
[feature d3451af] test message
 1 file changed, 5 insertions(+)
m-88888888:trainning_git hachi$ git commit --amend
hint: Waiting for your editor to close the file... error: There was a problem with the editor 'vi'.
Please supply the message using either -m or -F option.
m-88888888:trainning_git hachi$ git commit --amend
[feature 4b2dc68] コミット修正後
 Date: Sun Nov 10 19:08:59 2019 +0900
 1 file changed, 5 insertions(+)
 ```

 ## tag
 リリースバージョンなどの重要なタイミングで印をつけるためのもの。

 pushするときはtagをつけた段階でブランチの状態が、リモートリポジトリのreleaseに保存される。

 ## pull request
 Hello, Pull Request
 
PRテスト2

## PRフロー
issue -> branch -> 開発 -> push -> pull request