# 統合版サーバーからワールドをダウンロードする方法【Bedrock Edition】
### ※完全自己責任です。また<u>新たに追加されているブロックなどはすべて荒い土に置き換えられます</u>

## 紹介するプラットフォーム
- Windows

- ※おそらくjavaと両方のマイクラが動く環境なら可能

## 必要なもの
- javaのアカウント
- 統合版のアカウント

## 前提条件
- modを導入する知識があること(fabric)

### 0. Microsoft storeからje2beを入れておく（サイト版でも可能）
- (https://apps.microsoft.com/detail/9PC9MFX9QCXS?hl=ja-jp&gl=JP&ocid=pdpshare)

### 1. Viaproxyの設定

1. viaproxyをダウンロード
- ここから"viaProxy-3.x.x-SNAPSHOT.jar"ダウンロード(https://build.lenni0451.net/job/ViaProxy/)
- （できれば新しくフォルダを作るとなお良い）
- ※.jarを開けるようjavaを事前に入れておく

2. viaproxyを開く(開けない場合batファイルを使用すると開ける可能性があります)

3. アカウントを追加する

- 統合版アカウントを押してブラウザでログインする
- (必要であれば日本語にする)

4. 詳細設定で「パケットの変換エラーを無視」「リソースパックを受け入れたと偽装する」にチェックをいれる
### 2. Viaproxyの起動
1. サーバーアドレスの欄にアドレスを入れる
- このとき”IPAddres:Port”のようにいれる（"は不要）
2. サーバーバージョンの欄を「Bedrock 1.21.x」にする(または統合版最新)
3. Minecraftアカウントの欄を「選択したアカウントを使用する」にする
4. 下の起動を押す
5. 下の画像のように表示されれば成功

### 3. マイクラの構成を作る
1. 1.21.4 fabricの構成を作る(推奨)
2. modを導入する
#### 必須Mod
- Cloth Config API (https://www.curseforge.com/minecraft/mc-mods/cloth-config/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)
- Fabric API (https://www.curseforge.com/minecraft/mc-mods/fabric-api/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)
- Fabric Launguage Kotlin (https://www.curseforge.com/minecraft/mc-mods/fabric-language-kotlin/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)
- WorldTools:World Downloader (https://www.curseforge.com/minecraft/mc-mods/worldtools/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)
### 4. サーバーのワールドをダウンロードする
1. マイクラを起動してサーバーを追加
- ip: 127.0.0.1:25568
- ※ここは起動した際に出たやつ
2. サーバーに参加した後目的のマップに行く
3. ESCを押しWorldToolsを押し上の欄に名前を入れてstart downloadを押す
4. このときダウンロードしたいすべてのチャンクが読み込まれるように動く
5. すべて読み込めたらESCを押して"save capture of {名前}"を押す
6. そうしたらシングルワールドで先程ダウンロードしたワールドがあるので読み込む
- その時葉っぱなどの自然に壊れるブロックがある場合は入ってすぐに"/tick freeze"を実行し"/gamerule randomTickSpeed 0"を実行しておく
7. ワールドを保存して退出
### 5. ワールドを統合版用に変換
1. "java版から" と "統合版に" を選択して次へを押す
2. 他のフォルダを選択で先ほどダウンロードしたワールドを開く
3. 開始を選択
4. mcworld 形式で保存を選択

### 6. 統合版でワールドを読み込む
1. mcworldを開いてワールドを読み込む（または展開してワールドフォルダにコピー）
2. ワールドを開いて完了！