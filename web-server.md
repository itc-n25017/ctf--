webサーバーのインストール

１.インストール
・sudo apt update
・sudo apt install apache2 

２.Apacheを起動
・sudo systemctl start apache2

３.動作確認
サービスの確認
・sudo systemctl status apache2
ブラウザで確認
・http://localhost

番外編
コンテンツの変更
１公開ディポジトリに移動
・cd /var/www/html
その中のapache2のファイルを編集
