# linux-drill

「ネットワークの構築と運用」で使う、Linux基本コマンドの30分ドリル用スクリプトです。
対象コマンド：pwd / cd / ls / mkdir / touch / cat / cp / mv / rm / chmod

## 使い方（Raspberry Pi で実行）

```
cd ~
wget https://meio-hi-iot.github.io/linux-drill/setup.enc
openssl enc -d -aes-256-cbc -pbkdf2 -a -in setup.enc -out setup.sh
bash setup.sh
```

- `setup.enc` は暗号化されています。復号のパスワードは授業で伝えます。
- 演習用ディレクトリ `~/drill` と、確認スクリプト `~/check.sh` が作られます。
- 答え合わせ：`bash ~/check.sh`（表示された内容を、Teams の授業チームの課題の Forms に入力して提出します）
- ステージを最初の状態に戻す：`bash ~/setup.sh 番号`（例：`bash ~/setup.sh 4`）
- `sudo` は付けずに、自分のユーザで実行してください。

## ファイル

- `setup.enc`：演習用スクリプト（暗号化済み）
