注意点

この操作はwindows11, Minecraft java edition想定です[統合版では動きません]

この操作はlan解放、ポート開放不要です

対応
minecraft 26.1.2 (java)

必要ファイル↓

paper 26.1.2 

https://fill-ui.papermc.io/projects/paper/family/26.1

magic 

https://www.spigotmc.org/resources/magic.1056/

必要環境↓

java 25 

https://adoptium.net/ja/temurin/releases

JDK 25 - LTSタブを押し

Temurin jdk-25.0.3+9, Windows 64 bit (.MSI)をダウンロード、インストールしてください

前提操作

ダウンロードしたjavaをインストールしてください（してない場合）

エクスプローラーを開き”表示”タブを押す出てきた画面の”表示”タブを押すファイル名拡張子にチェックを入れる

導入手順
1. sever-setupフォルダを作る
2. paper-26.1.2-72.jarをsever-setupフォルダに入れる(72は変わる可能性がある)
3. 右クリック→新規作成→テキストドキュメントで新規テキストドキュメント.txtができる
4. 新規テキストドキュメント.txtを開き

@echo off

java -Xms1G -Xmx2G -jar paper-26.1.2-72.jar nogui

pause

と入れて保存する(72は変わる可能性がある)

5. 新規テキストドキュメント.txtの名前をstart.batに変更する

6. start.batを起動する

7. このアプリがプライベートネットワークで通信することを許可しますかの様な警告は許可を押す

8. Failed to load eula.txtもしくはYou need to agree to the EULA in order to run the server. Go to eula.txt for more info.とコンソールに出てきたらコンソール（黒い画面）を閉じる

9. eula.txtを開き

10. eula=falseをeula=trueに書き換え保存する

11. サーバーコンソールでstopと入れサーバーを終了

12. pluginsフォルダにmagicを入れる

13. start.batを起動する

14. magic-weapon-pack.zipを解凍

15. plugins/magic/spellにmagic-weapon-pack内のspellフォルダ内のymlファイルを入れる

16. plugins/magic/wandにmagic-weapon-pack内のwandフォルダ内のymlファイルを入れる

17. minecraftをバージョン26.1.2で起動する

18. マイクラのマルチプレイ→サーバーの追加、サーバーアドレスにlocalhostと入れる

19. サーバーコンソールでop マイクラのユーザー名 と入れる

20. サーバーを再起動する（コンソールでstopと入れstart.batを起動しなおす）

21. /mgive 武器idと入れると武器を入手可能（武器IDは説明書に記載）

22. 説明書通りに動かそう！

よくある失敗
eula.txtの中身のeula=falseをeula=trueに書き換えてない
start.batがstart.bat.txtになってないかの確認
マイクラのバージョン違い
