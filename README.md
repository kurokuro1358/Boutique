# ブティック　ウェブサイト
- ## アプリの概要について  
    - ### __開発背景__　　
        コロナ禍で来店者数の減少に伴い、家にいながらもお店の商品を観覧できるようにするために、母親から依頼を受けてこのホームページを作成しました。
    - ### __開発期間__
        １週間
    - ### __開発人数__  
        １人
    - ### __役割__
        設計、コーディング

- ## 使用言語・OSについて  
    - ### __使用言語__
        PHP 7.4.12  
        MySQL 5.7.32
    - ### __開発環境__
        MAMP 6.3

- ## 環境構築の手順  
    1. [MAMP](https://www.mamp.info/de/downloads/)をダウンロードする。  　　
    ![MAMPのダウンロード画面](https://dl.dropboxusercontent.com/s/w8x7xsr628gzjl4/mamp.png)

    2. MAMPを起動する。
    ![MAMPを起動した画面](https://dl.dropboxusercontent.com/s/91ka1f0bsgxczvt/startMamp.png)

    3. MAMPの起動画面から、Preferences -> Server -> Choose... からDocument rootに作業ディレクトリを選択し、OKを押す。
    ![Document rootをカレントディレクトリに設定する画面](https://dl.dropboxusercontent.com/s/xkvse72e6sd79x1/setMamp.png)

    4. ホーム画面から右上のStartを押し、サーバーを起動する。デェフォルトでは、ポート番号は8888に設定してある。詳細は、Preferences -> Portsから確認できる。
    ![ポート番号を確認できる画面](https://dl.dropboxusercontent.com/s/vgnjhfz2li1ktgx/Server.png)
    
    5. Google Chromeを開き、[http://localhost:8888/phpmyadmin/](http://localhost:8888/phpmyadmin/)にアクセスする。
    ![phpMyAdmin](https://dl.dropboxusercontent.com/s/yjw28eixqkdvdz6/phpmyadmin.png)

    6. ユーザーアカウント -> ユーザーアカウントを追加する から新たにユーザーアカウントを作成し、グローバル特権に全てチェックする。  
    ユーザー名：kurokuro   
    ホスト名：localhost  
    パスワード：secret

- ## デモ
    1. サーバーを起動した状態で、[http://localhost:8888/](http://localhost:8888/)にアクセスする。  
    ![ホーム画面](https://dl.dropboxusercontent.com/s/fhth4yfqy6gwf1k/index.png)  

    2. ページ右上のページ管理より、IDとパスワードを入力して、ログインする。  
    ID:gest0000  
    パスワード:0000  

    3. ログインをすると、在庫の追加・編集・削除ができる。

    4. 在庫の追加・追加・編集により、[http://localhost:8888/catalog.php](http://localhost:8888/catalog.php)、[http://localhost:8888/coordinate.php](http://localhost:8888/coordinate.php)に編集結果が反映される。

- ## 注意した機能や工夫した点  
    - 在庫管理をプログラムを書かなくても、動的に変更できるようにしました。  
    - カタログページでは、商品の種類ごとで分けて閲覧できるようにしました。ユーザーが求めるものをすぐに、見つけられるようになりました。
    - スマートフォンから、このサイトを見る人が多いことから、スマートフォンでの見た目を重視して、サイトをデザインしました。
    - よく使う機能に関しては、関数としてまとめ、template.phpにまとめました。

- ## 注意点  
    - ページ管理画面で、在庫の追加・編集・削除をする場合に、エラーが出力される場合がありますが、動作は正常に行われているので、ご了承ください。
    - 選択する画像は、jpeg形式のものしか選択できないので注意してください。jpeg以外でも、投稿はできますが、ホーム画面で、正常に画像が表示されない場合があります。

