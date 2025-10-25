# Antique Optimizations For RTM
・RealTrainMod 1.7.10（KaizPatch）と公式ランチャーに対応する軽量化modpack。  
・多数のModとConfig変更を簡単に導入することが出来ます。
## 推奨環境
・Java 8.0.462+8（Eclipse Temurin）https://adoptium.net/temurin/releases?version=8&mode=filter&os=any&arch=any  
・Forge 10.13.4.1614  
・KaizPatch v1.9.3  
## 非互換性
・CodeChickinCore（Lib）とProjectRedの前提mod：GTNH版に変える。  
https://modrinth.com/mod/codechickencore-unofficial/versions  
https://modrinth.com/mod/codechickenlib-unofficial/versions  
https://github.com/GTNewHorizons/ForgeMultipart/releases  
https://github.com/GTNewHorizons/ForgeRelocationFMP/releases  
https://github.com/GTNewHorizons/ForgeRelocation/releases  
https://github.com/GTNewHorizons/MrTJPCore/releases  

・WebCTC：CodeChickinCore Unofficialに未対応のため、AngelicaやFalsePatternLibと併用不可。また、ArchaicFixと相性が悪いらしい。  
WebCTCを使いたい場合はこちらを参考に。  
https://madoha-4862.hatenablog.jp/entry/2024/09/11/231348#%E3%83%BC%E6%A7%8B%E6%88%90%E3%83%BC  

・純正RealTrainMod（？）：倉急ワールドにて看板の描画時にぬるぽでクラッシュするバグが確認されたが原因不明。  

・KaizPatch：Beddium版でfalsetweaks.cfgのthreadedChunkUpdatesを有効にしていると、純正⇒KaizPatchに移行したワールドの架線柱モデルがバグる。先述の設定を無効化するか、移行後に架線柱モデルを全て置き直す。  

・純正＆KaizPatch：一部のレールが黒くなるバグの対策でLumiを入れているが、Lumiを入れているとトンネル内の一部レールが1.12.2のように明るくなる。  

・Liteloader：Angelica等と競合するのでLiteloaderLoaderを導入。https://modrinth.com/mod/liteloaderloader  

・OptiFine：OptiFineを使わない想定で制作しているので、無理矢理入れると不具合の原因になる。
## 注意事項
・jarファイルは自動で置き換えられないので、導入前に既存の軽量化modやそれらの前提mod、ID拡張modを全て削除してください。  

・軽量化の記事にあるBeddium構成とAngelica構成を元に、いくつかmodが追加されています。  
https://madoha-4862.hatenablog.jp/entry/2024/09/11/231348  

・falsetweaks.cfgのthreads（チャンクロードに使うCPUのスレッド数）をデフォルトで最大の8スレッドにしています。使っているCPUのコア数（スレッド数）が少ない場合は値を小さくしてください。  

・「Realms」「LANに公開」「配信設定」「Super Secret Settings」のボタンが削除されます。また、自分にかかっているポーションのパーティクルが見えないようになります。
## Angelica版とBeddium版、どちらが良いか
・チャンクロード速度：Beddium（マルチスレッド）≧ Angelica > Beddium（シングルスレッド）> OptiFine
・影の互換性：OptiFine > SwanSong > Angelica
・リソースパックの互換性：OptiFine > RightProperMCPatcher > Angelica
## 導入方法
・ReleaseからZipをダウンロードして、解凍する。  
・「Config」フォルダを既存のConfigフォルダに上書きする。  
・既存の軽量化modやID拡張modを削除。
・FileDirectorをダウンロードし、modsに入れる。  
https://modrinth.com/mod/filedirector/versions?g=1.7.10  
・起動するとmodのダウンロード画面が出てくるので、「NEXT」を押してダウンロード。  
・警告画面が出たら✕ボタンでMinecraftを終了。クラッシュしたらそのまま次へ。  
・FileDirectorはもう要らないので削除。  
・Minecraftを再起動。  
・導入完了。  
## Modリスト
https://madoha-4862.hatenablog.jp/entry/2025/10/25/120306
## ライセンス
LGPL3。ライセンスの全文はmodpackのZip内のreadme.txtにあります。
## クレジット（Configファイル）
Angelica by GT:NewHorizons  
https://github.com/GTNewHorizons/Angelica?tab=License-1-ov-file#readme  
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
SwanSong by vfx-dev  
https://github.com/vfx-dev/SwanSong?tab=License-1-ov-file#  
