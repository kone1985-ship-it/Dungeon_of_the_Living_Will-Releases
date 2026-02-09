Dungeon of the Living Will（配布用）

■最初に
- 同梱の「DungeonTools.exe」を起動してください。
- 「設定」ページで「APIキー」「モデル名」「Base URL」「画像生成モデル(任意)」を入力してください。
- 推奨設定は下記のとおりです。
    - APIキー： 下記で発行したもの
        -「https://console.x.ai/home」から sign in もしくは create account する
        - console が開くので、左のメニューから「API Keys」を選択
        - 適当な名前を入力して、create API key を押す
        - API key が発行されるので、それを「APIキー」に入力。
        - 左のメニューから Dashboard を選択し Puerchase をクリック もしくは
        　画面上部に「You have no paid credits」と出るのでクリック
        - 課金額を入力。最初は $5 で十分。
        - 「Add your first card」 を押して支払情報を登録
    - モデル名： grok-4-1-fast-reasoning
    - Base URL： https://api.x.ai/v1
    - 画像生成モデル定義： grok-2-image-1212
    - 最後に「保存」をクリック

■ ゲーム起動方法
- 「Dungeon_of_the_Living_Will/Dungeon_of_the_Living_Will.exe」を実行してください。
- 「Dungeon_of_the_Living_Will/_internal」フォルダは同じ場所に必要です（削除/移動しないでください）。

■ よくあるトラブル
- 起動しても何も出ない：ウィンドウ生成まで数秒かかる場合があります。しばらく待ってください。
- セキュリティ警告：配布形態によっては SmartScreen 等が警告を出すことがあります。

■ 備考
- 本ビルドは PyInstaller（onedir）で作成されています。
