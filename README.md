# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？
- リモートリポジトリは、ネット上に配置したリポジトリ（ファイルやディレクトリの状態を記録する場所）のことで、記録したデータを複数人で共有できる。
- ローカルリポジトリは、自身のPC内に配置したリポジトリのことで、変更を加えたデータなどをPC内に保存しておけるため、開発者個々人が手元のPCで開発を行うことができる。

## プッシュとマージの違いは何でしょうか？
- コミット（変更履歴を保存）した編集データを反映させる方法と場所が異なる。
  - プッシュは、ローカルリポジトリ内でコミットした編集データをリモートリポジトリに反映させる。
  - マージは、作業ブランチでコミットした編集データをマスター（メイン）ブランチに取り込んで反映させる。

## コミットとプッシュの違い
- コミットは編集データの変更した履歴を保存する操作で、プッシュはそのコミットしたデータをリモートリポジトリに反映させる操作。


## コミットのメッセージはどのように書いてあげるのが最適でしょうか？
- 簡潔にまとめ、かつ一目見て分かる内容にする。


## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？
- ローカルとプルリクエストでは取り込むまでの早さとデータの安全性が異なる。
  - ローカルでマージするときは、すぐにマスターブランチにコミットした内容を取り込むことができる。
  - プルリクエストでマージするときは、プルリクエストを作成してほかの人に変更した内容をレビューしてもらった後にマージしてもらうため、ローカルよりもマージまでに時間はかかるが、その分確認作業が入るためバグの混入を防げる。


## コンフリクトを起こしてしまった場合、どう対処すべきですか？
- ３つの対処方がある。
  - 先にマージした変更内容を取り込む。
  - 後にマージする予定の変更内容を取り込む。
  - 両方の変更内容を取り込んだ処理で上書きすることで、両方とも取り込む。
