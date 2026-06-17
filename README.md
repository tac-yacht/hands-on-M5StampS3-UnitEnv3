# hands on M5 StampS3 with Unit ENV-III

M5 StampS3 を MicroPythonで SORACOM に接続するハンズオン手順書のリポジトリです。  
M5 StampS3 については [製品ページ](https://docs.m5stack.com/ja/core/Stamp-S3A_PIN127) を参照してください。

## ハンズオン全体像

- 環境構築 (Thonny インストール / 10 分)
- hello, world で L チカ (5 分)
- SIM の開通と Harvest の ON (10 分)
- SORACOM へのデータ送信、Harvest で確認 (10 分)
- センサーをつないで試す（5 分)
- あとかたづけと注意事項 (5 分)

## 用意する物

- [StampS3A PIN1.27（1.27mmピッチピンヘッダ実装済）](https://docs.m5stack.com/ja/core/Stamp-S3A_PIN127)
  - ピンヘッダ実装の違いに注意してください。後述のBreakoutと接続できなくなります。
  - 旧版でもおそらく問題ありませんが、サポート対象外です。
- [StampS3 GroveBreakOut（1.27 mmピッチピンソケット実装済）](https://docs.m5stack.com/en/accessory/StampS3%20GroveBreakOut)
  - ブレッドボード等を介して接続する場合はこの限りではありません。本ハンズオンでは半田付けなしとしています。
- [Unit ENV-III](https://docs.m5stack.com/ja/unit/envIII)
- USB Type-Cケーブル
  - 片方はType-CでM5Stampとの接続でき、もう片方はPCにつなげるケーブルを用意してください。

## ドキュメント

- [ハンズオン目次](./docs/README.md)

## 著作権
本ドキュメントは、[hands-on-microcat1](https://github.com/soracomug/hands-on-microcat1.git)の派生です。
オリジナルライセンスは、[派生元ライセンス](hands-on-microcat1_LICENSE)をご確認ください。

## 謝辞
ハンズオンを公開してくださってるSORACOM UGの皆様、ありがとうございます。

author:TAC_yacht
