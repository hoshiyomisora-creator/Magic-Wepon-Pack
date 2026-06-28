#注意点

この操作はwindows11, Minecraft java edition想定です[統合版では動きません]

この操作はlan解放、ポート開放不要です

#対応
minecraft 26.1.2 (java)

#必要ファイル↓

paper Minecraft.V26.1.2用 

https://fill-ui.papermc.io/projects/paper/family/26.1

magic 

https://www.spigotmc.org/resources/magic.1056/

#必要環境↓

java 25 

https://adoptium.net/ja/temurin/releases

JDK 25 - LTSタブを押し

Temurin jdk-25.0.3+9, Windows 64 bit (.MSI)をダウンロード、インストールしてください

#前提操作

ダウンロードしたjavaをインストールしてください（してない場合）

エクスプローラーを開き”表示”タブを押す出てきた画面の”表示”タブを押すファイル名拡張子にチェックを入れる

#導入手順
1. server-setupフォルダを作る

2. ダウンロードしたpaper-26.1.2-xx.jarの名前をpaper.jarに変える

3. paper.jarをserver-setupフォルダに入れる

4. 右クリック→新規作成→テキストドキュメントで新規テキストドキュメント.txtができる

5. 新規テキストドキュメント.txtを開き

@echo off

java -Xms1G -Xmx2G -jar 

paper.jar nogui

pause

と入れて保存する

5. 新規テキストドキュメント.txtの名前をstart.batに変更する

6. 警告は許可

7. start.batを起動する

8. 警告は許可

9. このアプリがプライベートネットワークで通信することを許可しますかの様な警告は許可を押す

10. Failed to load eula.txtもしくはYou need to agree to the EULA in order to run the server. Go to eula.txt for more info.とコンソールに出てきたらコンソール（黒い画面）を閉じる

11. eula.txtを開き

12. eula=falseをeula=trueに書き換え保存する

13. pluginsフォルダを探す

14. pluginsフォルダにmagicを入れる

15. start.batを起動する

16. サーバーコンソールでstopと入れサーバーを終了

17. magic-weapon-pack.zipを解凍

18. pluginsフォルダを開いてmagicフォルダを探し開く

19. magicフォルダ中にspell,wandがあることを確認

20. spellを開きmagic-weapon-pack内のspellフォルダ内のymlファイルを入れる

21. wandを開きmagic-weapon-pack内のwandフォルダ内のymlファイルを入れる

22. minecraftをバージョン26.1.2で起動する

23. マイクラのマルチプレイ→サーバーの追加、サーバーアドレスにlocalhostと入れる(自分のIPではなく"localhost"と入れる)

24. サーバーコンソールでop マイクラのユーザー名 と入れる

25. サーバーを再起動する（コンソールでstopと入れstart.batを起動しなおす）

26. /mgive 武器idと入れると武器を入手可能（武器IDはweapons.mdに記載）

#リソースパックの導入（見た目の変更）

1. マインクラフトランチャーを起動する

2. 起動構成タブをクリック

3. ”プレイ”と書いてあるボタンの右側のフォルダマークを押す

4. 出てきたエクスプローラーウィンドウからresourcepacksフォルダを探す

5. resourcepacksフォルダを開く

6. 中にMagic-Weapon-Pack-Resourcepackフォルダをコピー

7. マインクラフトを起動する

8. 起動後→設定→リソースパック→利用可能タブからMagic-Weapon-Pack-Resourcepackを選択中に移動

#確認
□ java25を入れた

□ マインクラフトージョンが会っている

□ paperのバージョンが会っている

□ eula=trueとなっている

□ start.batがstart.bat.txtになってないかの確認

□ サーバーアドレスにlocalhostと入れる

#よくある失敗

#サーバーが起動しないorサーバーに入れない

magic.jar paper.jarを解凍している(してはいけない)

eula.txtの中身のeula=falseをeula=trueに書き換えてない

start.batの中身のミス

start.batがstart.bat.txtになってないかの確認

手順6.8.9で許可を押してない

マイクラのバージョン違い
