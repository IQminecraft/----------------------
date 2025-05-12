# 統合版サーバーからワールドをダウンロードする方法【Bedrock Edition】

### ※完全自己責任です。私は一切の責任を負いません。
### また<u>新たに追加されているブロックなどはすべて荒い土に置き換えられます</u>

## 紹介するプラットフォーム
- Windows
  ※おそらくJavaと両方のマイクラが動く環境なら可能

## 必要なもの
- Javaのアカウント
- 統合版のアカウント

## 前提知識
- MODを導入する知識（Fabric）
- Javaと統合版でのワールド導入に関する知識

## やり方

### 0. Microsoft Storeからje2beを入れておく（サイト版でも可能）
- [je2beのダウンロードリンク](https://apps.microsoft.com/detail/9PC9MFX9QCXS?hl=ja-jp&gl=JP&ocid=pdpshare)

### 1. Viaproxyの設定

1.  **Viaproxyをダウンロード**
    -   ここから"viaProxy-3.x.x-SNAPSHOT.jar"をダウンロード: [Viaproxyダウンロードリンク](https://build.lenni0451.net/job/ViaProxy/)
    -   （できれば新しくフォルダを作るとなお良い）
    -   ※.jarを開けるようにJavaを事前にインストールしておく
2.  **Viaproxyを開く**
    -   開けない場合はbatファイルを使用すると開ける可能性があります。
3.  **アカウントを追加する**
    -   統合版アカウントを押してブラウザでログインする
    -   (必要であれば日本語に設定する)
        ![image1](https://github.com/IQminecraft/how_to_download_a_map_from_bedrock_servers/blob/main/images/image1.png)
4.  **詳細設定**
    -   「パケットの変換エラーを無視」「リソースパックを受け入れたと偽装する」にチェックを入れる

### 2. Viaproxyの起動
1.  **サーバーアドレスの欄にアドレスを入力**
    -   このとき"IPAddres:Port"の形式で入力（"は不要）
2.  **サーバーバージョンの欄を設定**
    -   「Bedrock 1.21.x」（または統合版最新）を選択
3.  **Minecraftアカウントの欄を設定**
    -   「選択したアカウントを使用する」に設定
4.  **下の起動を押す**
5.  **成功の確認**
    -   下の画像のように表示されれば成功

### 3. マイクラの構成を作る
1.  **1.21.4 Fabricの構成を作成（推奨）**
2.  **MODを導入する**

#### 必須Mod
-   [Cloth Config API](https://www.curseforge.com/minecraft/mc-mods/cloth-config/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)
-   [Fabric API](https://www.curseforge.com/minecraft/mc-mods/fabric-api/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)
-   [Fabric Language Kotlin](https://www.curseforge.com/minecraft/mc-mods/fabric-language-kotlin/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)
-   [WorldTools: World Downloader](https://www.curseforge.com/minecraft/mc-mods/worldtools/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)

### 4. サーバーのワールドをダウンロードする
1.  **マイクラを起動してサーバーを追加**
    -   IP: `127.0.0.1:25568`
    -   ※ここは起動した際に表示されたもの
2.  **サーバーに参加した後、目的のマップに移動**
3.  **ESCを押してWorldToolsを選択**
    -   上の欄に名前を入力して「start download」を押す
        ![image2](https://github.com/IQminecraft/how_to_download_a_map_from_bedrock_servers/blob/main/images/image2.png)
4.  **ダウンロードしたいすべてのチャンクが読み込まれるように動く**
5.  **すべて読み込めたらESCを押して「save capture of {名前}」を押す**
6.  **シングルワールドで先程ダウンロードしたワールドを読み込む**
    -   その時、葉っぱなどの自然に壊れるブロックがある場合は入ってすぐに`/tick freeze`を実行し`/gamerule randomTickSpeed 0`を実行しておく
7.  **ワールドを保存して退出**

### 5. ワールドを統合版用に変換
1.  **"java版から" と "統合版に" を選択して次へを押す**
2.  **他のフォルダを選択で先ほどダウンロードしたワールドを開く**
3.  **開始を選択**
4.  **mcworld形式で保存を選択**
    ![image3](https://github.com/IQminecraft/how_to_download_a_map_from_bedrock_servers/blob/main/images/image3.png)

### 6. 統合版でワールドを読み込む
1.  **mcworldを開いてワールドを読み込む（または展開してワールドフォルダにコピー）**
2.  **ワールドを開いて完了！**

## さいごに
### 特に許可されてないサーバーなどでの使用は自己責任です
#### 自分が体験したこと書いときます
-   ブロックをおいたり壊したりすると蹴られる（非対応）な部分がある
-   右クリックアイテムが反応しなかったりチェストになってる場合はめんどいけど他の方法でワールドに入るしかない
-   新たに追加されてるブロックが多い場合は使えない（すべて荒い土になるため）
-   経由サーバーなどがある場合はhorionでサーバーのIPとPORTを取っておくと楽
-   Hiveは直IPじゃないと入れないので貼っときます -> `139.99.116.122:19132`
