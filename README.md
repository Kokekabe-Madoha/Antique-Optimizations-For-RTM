# Antique Optimizations For RTM
・RealTrainMod 1.7.10（KaizPatch）と公式ランチャーに対応する軽量化modpack。  
・多数のModとConfig変更を簡単に導入することが出来ます。
## 推奨環境
・Java 8.0.462+8（Eclipse Temurin）https://adoptium.net/temurin/releases?version=8&mode=filter&os=any&arch=any  
・Forge 10.13.4.1614  
・KaizPatch v1.9.3  
## 非互換性
・WebCTC：CodeChickinCore Unofficialに未対応のため、AngelicaやFalsePatternLibと併用不可。また、ArchaicFixと相性が悪いらしい。  
WebCTCを使いたい場合はこちらを参考に。  
https://madoha-4862.hatenablog.jp/entry/2024/09/11/231348#%E3%83%BC%E6%A7%8B%E6%88%90%E3%83%BC  
・純正RealTrainMod（？）：倉急ワールドにて看板の描画時にぬるぽでクラッシュするバグが確認されたが原因不明。  
・KaizPatch：Beddium版でfalsetweaks.cfgのthreadedChunkUpdatesを有効にしていると、純正⇒KaizPatchに移行したワールドの架線柱モデルがバグる。先述の設定を無効化するか、移行後に架線柱モデルを全て置き直す。  
・純正＆KaizPatch：一部のレールが黒くなるバグの対策でLumiを入れているが、Lumiを入れているとトンネル内の一部レールが1.12.2のように明るくなる。  
・Liteloader：Angelica等と競合するのでLiteloaderLoaderを導入。https://modrinth.com/mod/liteloaderloader  
## 注意事項
・jarファイルは自動で置き換えられないので、導入前に既存の軽量化modを全て削除してください。  
・軽量化の記事にあるBeddium構成とAngelica構成を元に、いくつかmodが追加されています。  
https://madoha-4862.hatenablog.jp/entry/2024/09/11/231348  
・falsetweaks.cfgのthreads（チャンクロードに使うCPUのスレッド数）をデフォルトで最大の8スレッドにしています。使っているCPUのコア数（スレッド数）が少ない場合は値を小さくしてください。
## 導入方法
・ReleaseからZipをダウンロードして、解凍する。  
・「Config」フォルダを既存のConfigフォルダに上書きする。  
・FileDirectorをダウンロードし、modsに入れる。  
https://modrinth.com/mod/filedirector/versions?g=1.7.10  
・起動するとmodのダウンロード画面が出てくるので、「NEXT」を押してダウンロード。  
・タイトル画面まで行くか、警告画面が出たら、一旦Minecraftを終了。  
・FileDirectorはもう要らないので削除。  
・Minecraftを再起動。  
・導入完了。  
