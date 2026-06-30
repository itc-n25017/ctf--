ftpサーバーのインストール

１.インストール
・sudo apt update
・sudo apt install vsftpd 

２.起動
・sudo systemctl start vsftpd

３.起動確認
・sudo systemctl status vsftpd

４.設定ファイル
　設定ファイルを開く
・sudo vi /etc/vsftpd.conf
　項目の変更
・anonymous_enable=No
  local_enable=YES
  write_enable=YES
  local_umask=022

５.接続確認
　ローカルから接続
・ftp localhost
　別PCから接続
・fpt {サーバーのIPアドレス}

6.ポートが空いているか確認
ss -lntp | grep :21
