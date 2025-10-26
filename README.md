## OpenDolphin-2.7.3m-client

### 概要
OpenDolphin-2.7.3m (2.7m) は、 dolphin-dev/OpenDolphin のオープンソース電子カルテ OpenDolphin2.7.0b (2.7) の modified version（ bugfix + α）です。
 * クライアント外観・データ構造は 2.7 と完全に同一です。
 * ファイルバックアップ機能を備えています。
 * Java17, JakartaEE10 環境での動作を確認しています。  
 いい加減、サーバーとクライアントは分離した方がいいと思い、本リポジトリにはクライアントに関係するソースコードのみ収載しています。  

### インストール方法

 * [OpenOcean/OpenDolphin をカスタマイズするために知っておいた方がよいこと](https://phazor.info/OpenOcean/?p=1)
 * [OpenOcean/OpenDolphin をカスタマイズするために知っておいた方がよいこと ２](https://phazor.info/OpenOcean/?p=217)
 * [Open Dolphin 2.7.0b を Win10 にインストールしてみた](https://phazor.info/air/?page_id=543)
 * [Open Dolphin 2.7(m) を Mac OSX にインストールする](https://allnightnihon2b.net/blog-jp/?page_id=367)

　などを参考にしてください。

### クライアント起動方法
Mac であれば、ダブルクリック一発で起動できるはずです。  
  
![opendolphin on JakartaEE, Java17](https://user-images.githubusercontent.com/8698703/200154977-39c4a66a-058d-40a5-b12d-d3bc1dc7aad2.png)
  
  
### 派生プロジェクト
[OpenOcean](https://github.com/air-h-128k-il/OpenOcean)が実質的な後継プロジェクトです。  
  
* 当プロジェクト fork 後、コードメンテナンスおよびいくつかの機能が追加されています。  
* さらに将来的に DICOMviewer/PACS [HorliX](https://github.com/air-h-128k-il/HorliX) との連携も期待できます。  
  
[OpenOcean](https://phazor.info/OpenOcean/) の利用も検討してみてください。  
と言っていたのですが OpenOcean 大幅書き直しの予定（→ [DolphORCA](https://p-horlix.net/blog/?page_id=346) プロジェクトに統合されました）なのでこちらを現役復帰させる（かも）。  
現在でも使えることは使えると思います。  
ただし、安全性に関するガイドラインの Ver5.2 以降、システム停止時には本系統とは「別に」見読性確保のためのビューアを設置することが推奨されています。 
   
![OpenDolphin HTML/PDF Viewer](https://i0.wp.com/p-horlix.net/blog/wp-content/uploads/2022/05/OpenDolphin_HTML_PDF_Viewer_inomata_air-h-128k-il.png?w=900&ssl=1)
  
2.7m 系列では [OpenDolphin HTML/PDF Viewer](https://p-horlix.net/blog/?p=289) が用意されています。  
こちらはオープンソースでもなんでもないため、本リポジトリには含まれていません。  
　　
### 著作権表記  
ややこしい。  
    

### OpenOcean 騒動
「OpenOcean は GPL に違反している！」と物騒な主張をする人が過去にいました。  
顛末は『[OpenOcean 怪文書](https://researchmap.jp/blogs/blog_entries/view/143851/cf29de114fa73c109536ac188d7e0345)』・『[小林慎治氏の OpenOcean に関する事実誤認](https://phazor.jp/blog/?p=336)』などにまとめてあります。  

  
### その他
Java17 移行が若干難しいかもしれません。  
これは、Java に加わった新機能「モジュール」に古いドルフィンのソースコードが対応していないためです。解決方法はいくつかあり、もっとも自然な方法は、邪魔になっている箇所を削除して同様の機能を実装することです。2.7m 系列では、既にこの作業を完了しています。が、このバージョンは単に JDK を 1.8 -> 17 としただけです。  
JakartaEE 10 への移行作業はこれに比べると単純ですが、修正する箇所はけっこうあると思います。
    
air-h-128k-il  

