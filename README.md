# README

## 環境構築
```
$ bundle install
$ bin/rails db:setup
$ yarn install
$ bin/rails s
```

## 事業をエンジニアリングしよう提案編の回答は以下に記述してください
選択した事業側の課題

サービス登録者数の内、男性60%に対して、女性は40%。一方で、サービス内のもくもく会に参加した人の比率は、男性90%：女性10%と大きな差が出ています。もっと女性が使いやすいようなサービス設計にする必要があるのではないか？



提案内容

もくもく会作成時に女性限定と設定、絞り込みができるようにする。
会場の写真等を一枚でなく複数載せられるようにする。
主催者の自己紹介欄をつくる。

→女性の方は現状のもくもく会だと参加しても少数派になりやすく、会に参加しにくいと思う。なのでタグを用意して女性限定のもくもく会が開きやすいようにする。また、絞り込みですぐに女性限定のもくもく会を見つけやすいようにする。
また会場がおしゃれかどうか、トイレ等の設備もわかりやすいと安心感が出るので画像を複数載せれるように。
主催者がどんな人かわからないと参加しにくい。なので、もくもく会の詳細欄から主催者名クリックで見れるようにする。



実装方針
＜女性限定＞←今回のこれのみ実装
・もくもく会作成時に女性専用のタグを指定できるようにする。タグはチェックボックスで女性限定のみ。
・ヘッダーにある検索フォームに女性限定タグの条件を追加する。
・一覧画面において、各イベントに付与されている女性限定タグをタップすると絞り込みが行われるようにする。

＜複数画像＞
・画像を複数入力(3枚まで)できるように入力フォームを変更する。
・もくもく会詳細画面にて複数画像を表示できるようにする。

＜主催者自己紹介＞
・もくもく会の入力フォームにて主催者自己紹介の入力欄を作成する
・もくもく会詳細画面にて主催者名をタップするとモーダルで自己紹介を表示できるようにしていく。