# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？

- リモートリポジトリとは、ネット上に配置するリポジトリのこと。複数人で共有するためのもの。

- ローカルリポジトリとは、PCに配置するリポジトリのこと。開発者それぞれが個人で使用するためのもの。

## プッシュとマージの違いは何でしょうか？

- プッシュは、ローカルリポジトリの変更をリモートリポジトリに反映させる。

- マージは、別のブランチの作業履歴を、現在のブランチへを統合する。

- プッシュはローカルリポジトリからリモートリポジトリへ更新内容を反映する際に使用すが、マージはローカルリポジトリ内で、作業ブランチの更新内容を主要なブランチへ反映する際に使用する。

## コミットとプッシュの違い

- コミットは、ローカルリポジトリで行った作業内容の履歴を、ローカルリポジトリに保存すること。

- プッシュは、ローカルリポジトリでコミットした変更を、リモートリポジトリにアップロードすること。

- プッシュはローカルリポジトリ内で行われる作業であり、プッシュはローカルリポジトリからリモートリポジトリへ対して行われる作業である。

## コミットのメッセージはどのように書いてあげるのが最適でしょうか？

- コミットメッセージは、その履歴がどんな編集を行なったのか、第三者から見て分かりやすいように記述する。

## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？

- プルリクエストとは、他の開発者にブランチの変更内容のマージを依頼すること。

- ローカルでマージする場合は、開発者によるマージにより、更新内容がそのまま主要ブランチへ統合される。ローカル作業ブランチからローカル主要ブランチへマージし、リモート主要ブランチへプッシュするフローになる。

- プルリクエストでマージする場合、レビュー担当者がコードレビューしてからマージするという段階を踏む。第三者によるコードレビューの手順挟むことで、ミスを防止するメリットがある。ローカル作業ブランチからリモート作業ブランチへプッシュし、コードレビューが承認されると、リモート主要ブランチへマージされるフローになる。

## コンフリクトを起こしてしまった場合、どう対処すべきですか？

 - コンフリクトが起きた時は、以下3通りの方法の中から、状況に応じた方法で変更を取り込む。

 1. 先にマージされた変更内容を取り込む
 2. 後にマージしようとしている変更内容を取り込む
 3. どちらの変更内容も取り込む