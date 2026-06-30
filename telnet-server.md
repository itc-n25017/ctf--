telnetサーバーのインストール

１．telnetサーバーをインストール
・sudo apt update
・sudo apt install openbsd-inetd telnetd

２．サービスを起動
・sudo systemctl start openhsd-inetd

３．サービスの状態を確認
・sudo systemctl status openbsd-inetd

４．Telnetの待ち受け確認
ss -lntp | grep :23

５．クライアントから接続
　ローカルで接続
・telnet localhost
　別PCから接続
・telnet {サーバーのIPアドレス}

