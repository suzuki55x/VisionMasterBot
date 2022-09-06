# VisionMasterBot

Discord上で動作する、Phantom Magic VISIONのカードテキスト表示BOT。

カードのデータは <http://coolier.dip.jp/th_up4/index.php?id=6445> にて配布されているデータを基に、JSON形式へ変換を行っております。

カードリスト編集を行った皆様へ、この場にて感謝を申し上げます。

また、このBotは[ここ](https://discord.com/api/oauth2/authorize?client_id=678036269133201410&permissions=120279197760&scope=bot)からサーバーへ追加できます。

---

## このリポジトリが存在する理由

このBOTは現在はうしりす（[twitter](https://twitter.com/ushirisu)）の自宅PCで運用しており、できる限り常に利用できるようにしております。

それでもWindowsの更新やBOTの更新作業などで落ちる事があるため、使いたいときに確実に使いたい！という方向けに、自身で同じBOTを作れるようにこのリポジトリを制作いたしました。

---

## このBOTを起動するためには

- JavaScriptについて、コンソールに文字を出せるぐらいの知識が必要です

- NodeJSについて、「"npm init"を実行したことがある」ぐらいの経験が必要です

---

## このBOTを編集・改良するためには

- JavaScriptでGET/POSTを行える程度の知識が必要です

- 自己満足で書かれた💩コードを許せる心の広さが必須です（重要）

---

## 必要なソフト・環境

- NodeJSが利用できる環境である（必須）

- VScodeが利用できる（推奨。制作者の環境がこれなので...）

- 上記2つの条件を満たせればOSはなんでもいいと思います

---

## 最初にやること

1. このリポジトリをダウンロード（もしくはクローン）する

1. DiscordのBOTを作成する（<https://techmel.net/discord-bot-intro/>等が参考になります）

1. `envioment.json`を作成し、ファイルの内容を`{"token" : "ここをBOTのトークンに置換"}`にする

1. `data\commandLog.json`を作成し、ファイルの内容を`{"log" : []}`にする

1. `data\premiumUser.json`を作成し、ファイルの内容を`{"guildList" : ["ここをサーバーIDに置換"]}`にする(推奨)

1. VScode（もしくはコンソール、PowerShellや"端末"など）でダウンロードしたフォルダを開く

1. コンソールで`npm i`を実行する（少し時間がかかります）

1. コンソールで`npm -g hotnode`を実行する

---

## 起動したいときにやること

1. VScode（もしくはコンソール、PowerShellや"端末"など）でダウンロードしたフォルダを開く

1. コンソールで`npm hotnode main.js`を実行する

---

## 仕様

- !ytや!bgmコマンドはPCへの負荷が高いため、利用可能なサーバーを限定できるようにしています（初期設定の3.がその設定です。）

- 実行したPCをサーバーとして使用するため、そのPCをシャットダウンするとオフライン状態（BOTが停止状態）になります。
