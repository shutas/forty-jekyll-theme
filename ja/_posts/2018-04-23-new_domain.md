---
layout: post
title: New Domain
description: 新しいドメイン名に変更しました
image: assets/images/2018-04-23.jpg
date: 2018-04-23 22:39:47
lang: ja
---

先週は大学の期末試験期間だったんですけど、気晴らしにこのウェブサイト用にドメイン名を購入しました。俗に言うアドレスってやつです。

もともとはこのサイトをデプロイしている[Netlify](https://netlify.com/){:target="_blank"}のサブドメインを使っていたんですけど、やっぱりせっかくの自分のウェブサイトなので個別のドメインが欲しい！と思い、買っちゃいました。その結果、皆さんご存知の通り現在は新しいカスタムドメインである[shutasuzuki.com/ja](https://shutasuzuki.com/ja/){:target="_blank"}にてサイトをアクセスできるようになりました。このドメイン名は[Google Domains](https://domains.google/){:target="_blank"}にて購入しました。僕が購入したドメイン名は年間で12ドルと、比較的安く手に入れることができました。

![Google Domain Screenshot](/assets/images/2018-04-23.jpg){:class="image main"}

(Check Outを押して支払い情報を入力するだけで即購入することができました。便利な時代ですね。)

デプロイ先のNetlify上のプロジェクトは別のドメインへの移行がメチャクチャ簡単です。NetlifyのDNSレコードに新しいドメイン名を登録したあと、Google Domains側でネームサーバーをちょこっといじるだけですぐに作業完了。あとはDNS情報がインターネットの隅々に更新されるまで数時間時間を置くだけ。個人的には数時間で終わりましたが、場合によっては一日程度かかるそうです。

最近流行り（？）に乗っかろうと思い、SSL/TLSの証明書を[Let's Encrypt](https://letsencrypt.org/){:target="_blank"}にて発行しました。通信が暗号化されることによってちょっとでもネットの安全な利用につながればなあ、なんて思ってみたり。余談ではありますが、実はこのLet's Encryptの開発者の一人に[Alex Halderman](https://jhalderm.com/){:target="_blank"}という僕が通っている大学の教授がいるんですけど、来学期Halderman教授のコンピュータセキュリティの授業の履修登録をつい先日しました。正直個人的にはすごく楽しみです。

ま、というわけで皆さんもウェブサイトを持っていてドメイン名を変えたいな、と考えている方はぜひ参考にしてみてください。