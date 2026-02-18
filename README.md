![dokodemo_buffer_thumb_anim](https://github.com/user-attachments/assets/36e6e39f-fb6c-41f5-9ca3-b2e8b4ee0a9a)

# どこでもバッファ

![](https://aviutl2-catalog-badge.sevenc7c.workers.dev/badge/v/zopty.DokodemoBuffer)

レイヤー間で映像を送受信できるカスタムオブジェクトを追加します

beta33にて動作確認済

# 導入手順

### [ここからインストール](https://aviutl2-catalog-badge.sevenc7c.workers.dev/package/zopty.DokodemoBuffer) または

1. [AviUtl2カタログ](https://github.com/Neosku/aviutl2-catalog) をインストール
2. `どこでもバッファ` を検索してインストール
3. 次回AviUtl2起動時に `このプラグイン・スクリプトを信頼して使用する` をクリック

### 手動導入

1. [このリンクを右クリックして別名で保存](https://github.com/zopty/DokodemoBuffer/raw/refs/heads/main/@どこでもバッファ.anm2)
2. AviUtl2の画面にD&D
3. `このプラグイン・スクリプトを信頼して使用する` をクリック

# 使い方

`どこでもバッファ` ラベル内に以下のエフェクトが追加されます:

### `入出力` エフェクト

- それぞれのオブジェクトには `ID` が指定されており、同じ `ID` が指定されたオブジェクト同士で送受信が行われます
  - `ID` が `0` のオブジェクトから送信された映像は、同じく `ID` が `0` のオブジェクトでのみ受信できます
- `ID` には任意の文字列を設定できます
  - 無効な `ID` が指定された場合は何もしません
- `動作モード` を切り替えることで、入力と出力を切り替えられます

### `遅延` エフェクト

- 指定したフレーム数だけ映像を遅延させます
  - 1オブジェクトあたり `フレーム数 x シーン解像度` に応じたメモリを必要とします

### `残像` エフェクト

- 指定した数の残像を表示します
  - 各残像は `遅延` で指定したフレーム数ずつ遅れて表示されます

# ライセンス

このプログラムは `BSD 3-Clause License` のもとで公開されています

詳しくは [LICENSE](LICENSE) をご覧ください
