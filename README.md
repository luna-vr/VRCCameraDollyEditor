# Camera Dolly Studio

AIで作成したWebツールです。
VRChatのカメラドリー（Camera Dolly）の軌道を作成するための、キーフレームJSON生成補助ツールです。

公開ページ： https://luna-vr.github.io/VRCCameraDollyEditor/

## 概要

- ブラウザだけで動作し、オフライン対応です。編集データが外部サーバーに送信されることはありません
- 3Dプレビュー／上面図（X–Z）／側面図（Z–Y）で軌道を確認しながら、キーフレームごとの位置・回転・ズーム・次地点までの時間を編集できます
- プリセット収録：横へ平行移動（Trucking）、前後移動（Push In）、上下移動（Boom）、半円軌道（Arc）
- 既存のJSONの読み込み、編集結果のJSONダウンロード／コピーに対応しています

## 使い方

1. 公開ページを開きます
2. プリセットを選ぶか、キーフレームを編集し、再生プレビューで動きを確認します（上面図の地点はドラッグでも移動できます）
3. 「JSONをダウンロード」で保存し、VRChatの カメラ → Dolly → Advanced → Import で、ファイルのフルパスを指定して読み込みます

※ VRChatのCamera DollyはVRC+が必要です。Windowsでインポートする際はOSCを有効にしてください。

## 注意

- VRChat非公式ツールです。VRChat本体でのインポート・描画結果は別途確認してください
- プレビューはキーフレーム間を直線・等速補間した概算表示です。VRChat側では Dolly の Path Type = Linear、Motion Control = Time、Easingなしにすると近い動きになります
