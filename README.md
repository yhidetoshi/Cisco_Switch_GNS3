# Cisco_Switch_GNS3
study cisco_switch memo

##### 検証環境(GNS3のセットアップ)
- GNS3をダウンロード&インストール
-> https://www.gns3.com/

- iOSをダウンロード
-> http://www.w7cloud.com/GNS3-IOS/c3745-adventerprisek.124-25d.bin


Ciscoコマンドメモ　
=======
|コマンド    |説明         |
|:-----------|:------------|
|# configure terminal|グローバルコンフィギュレーションモードへ|
|# exit|一つ前のモードへ|
|# enable|特権EXECへ移動|
|# show startup-config|設定変更してから設定保存されたコンフィグ確認|
|# sh running-config|コンフィグ確認|
|# copy running-config startup-config もしくは write memory|コンフィグ保存|


|# ?|可能なコマンド表示|


- Interface(0/0)にアドレスを付与
```
# configure terminal
(config)# interface FastEthernet 0/0
(config-if)# ip address 10.0.2.11 255.255.255.0
(config-if)# no shutdown
```

