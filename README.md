# Antique Optimizations For RTM
・KaizPatchXと公式ランチャーに対応する軽量化modpack。  
・多数のModとConfig変更を簡単に導入することが出来ます。
## Angelica版について
Angelica版は構成の変更により、modpack化する必要が無くなったので廃止しました。  
以下の記事を参考に導入してください。  
https://madoha-4862.hatenablog.jp/entry/2024/09/11/231348#1710-Angelica  
## 推奨環境
・Java 8.0.472+8（Eclipse Temurin）https://adoptium.net/temurin/releases?version=8&mode=filter&os=any&arch=any  
・Forge 10.13.4.1614  
・RealTrainMod v1.7.10.46、KaizPatchX v1.9.3  
## 非互換性
・CodeChickinCore（Lib）とProjectRedの前提mod：GTNH版に変える。  
https://modrinth.com/mod/codechickencore-unofficial/versions  
https://modrinth.com/mod/codechickenlib-unofficial/versions  
https://github.com/GTNewHorizons/ForgeMultipart/releases  
https://github.com/GTNewHorizons/ForgeRelocationFMP/releases  
https://github.com/GTNewHorizons/ForgeRelocation/releases  
https://github.com/GTNewHorizons/MrTJPCore/releases  

・NotEnoughIDs（Unofficialも含む）：EndlessIDsを使う。  
https://modrinth.com/mod/endlessids/versions  

・WebCTC：CodeChickinCore Unofficialに未対応のため、FalsePatternLibと併用不可。また、ArchaicFixと相性が悪いらしい。  

・純正RealTrainMod：Beddiumとの競合で、看板の描画時にぬるぽでクラッシュすることがある。  

・KaizPatch：Beddium版でfalsetweaks.cfgのthreadedChunkUpdatesを有効にしていると、純正⇒KaizPatchに移行したワールドの架線柱モデルがバグる。先述の設定を無効化するか、移行後に架線柱モデルを全て置き直す。  

・純正＆KaizPatch：一部のレールが黒くなるバグの対策でLumiを入れているが、Beddium版でLumiを入れているとトンネル内の一部レールが1.12.2のように明るくなる。  

・Liteloader：LiteloaderLoaderを入れる。https://modrinth.com/mod/liteloaderloader  

・OptiFine：OptiFineを使わない想定で制作しているので、無理矢理入れると不具合の原因になる。  

・LWJGL3ify：このmodpackはBeddiumのJava8版を使用するが、LWJGL3ifyを導入する場合はJava21版に変更する。  

・Neodymium Unofficial：既にサポート終了済み。入れると警告が出る。

## 注意事項
・falsetweaks.cfgのthreads（チャンクロードに使うCPUのスレッド数）をデフォルトで最大の8スレッドにしています。使っているCPUのコア数（スレッド数）が少ない場合は値を小さくしてください。  

・ワールド参加時にEndlessIDsとLumiがワールドを変更する警告が出るので、「はい」で進んで下さい。後でEndlessIDsやLumiを抜いてもワールドは壊れないので大丈夫です。  

・トンネル内のレールの一部が1.12.2のように明るくなることがあります。  
## AngelicaとBeddium版、どちらが良いか
・平均FPS：Angelica > Beddium ≧ OptiFine  
・チャンクロード速度：Beddium（マルチスレッド）> Angelica > Beddium（シングルスレッド）> OptiFine  
・影とRTMの互換性：OptiFine > SwanSong ≧ Angelica    
・リソースパックの互換性：OptiFine > RightProperMCPatcher > Angelica  
## 導入方法
・ReleaseからZipをダウンロードして、解凍する。  
・「Config」フォルダを既存のConfigフォルダに上書きする。  
・既存の軽量化modを削除。軽量化mod以外でUniMixinsを要求するmodは一旦抜く。  
・FileDirectorをダウンロードし、modsに入れる。  
https://modrinth.com/mod/filedirector/versions?g=1.7.10  
・起動するとmodのダウンロード画面が出てくるので、「NEXT」を押してダウンロード。  
・警告画面が出たら✕ボタンでMinecraftを終了。クラッシュしたらそのまま次へ。  
・FileDirectorはもう要らないので削除。一旦抜いたmodも入れる。  
・Minecraftを再起動。  
・導入完了。  

・Modを自分で導入して、Configだけ使用するのも良い。
## Modリスト
https://madoha-4862.hatenablog.jp/entry/2025/10/25/120306
## ライセンス
LGPL3。ライセンスの全文はmodpackのZip内のreadme.txtにあります。
## クレジット（Configファイル）
ArchaicFix by Embeddedt  
https://github.com/embeddedt/ArchaicFix?tab=License-1-ov-file#  
https://github.com/embeddedt/ArchaicFix?tab=LGPL-3.0-2-ov-file#  
CoreTweaks by makamys  
https://github.com/GTNewHorizons/CoreTweaks?tab=License-1-ov-file#  
FalseTweaks by FalseParttern  
https://github.com/FalsePattern/FalseTweaks?tab=License-1-ov-file#  
https://github.com/FalsePattern/FalseTweaks?tab=GPL-3.0-2-ov-file#  
https://github.com/FalsePattern/FalseTweaks?tab=LGPL-3.0-3-ov-file  
HodgePodge by GT:NewHorizons  
https://github.com/GTNewHorizons/Hodgepodge?tab=LGPL-3.0-1-ov-file#  
Lwjgl3ify by GT:NewHorizons  
https://github.com/GTNewHorizons/lwjgl3ify?tab=LGPL-3.0-1-ov-file#readme  
SwanSong by vfx-dev  
https://github.com/vfx-dev/SwanSong?tab=License-1-ov-file#  
