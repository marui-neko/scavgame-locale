
***

# Casualties Unknown (Scav Prototype) 日本語化

このリポジトリは、Casualties Unknown (Scav Prototype) の日本語翻訳ファイルを公開・配布するための場所です。

> [!WARNING]
> **注意：非公式のModツールです。導入はすべて自己責任で行ってください！**

***

## 📖 導入手順

### ⚠️ ゲームの保存場所に注意！
ゲームのフォルダパスに「日本語」が含まれていると、日本語化ツールが動作しません。
* ❌ NG： `C:\新規ファイル\CasualtiesUnknown`
* ⭕ 推奨： `C:\New_File\CasualtiesUnknown`


必ず**英数字のみのパス**に配置してください。


***


### 📥 導入ステップ

1. [**CU日本語化パック**](https://mega.nz/file/Sk8zjCpS#trtLGbzXT2KevjPsZhmRs0CQ7SyoID8j5jrRJP801aE)をダウンロード  
   必要ファイルがすべて入っています。ダウンロードして解凍してください。

2. **ゲームフォルダに配置**  
   解凍した中身すべてを、ゲームの実行ファイル（`CasualtiesUnknown.exe`）と同じフォルダに配置します。

3. **ゲーム起動＆設定**  
   すべての配置が終わったら、`CasualtiesUnknown.exe` からゲームを起動  
   自動的に日本語ファイルをダウンロードし、適応します。

***

## ⚙️ オプション設定

タイトル画面右下の**ぬいぐるみ**を長押しクリックすることで、各種設定メニューにアクセスできます。

### 🔄 日本語翻訳データのアップデート方法について 

翻訳データのアップデートには、2種類の方法が用意されています。

1. **公式リポジトリからダウンロード（安定版）**  
公式に承認された安定した翻訳データを使用する場合に推奨されます。
   * プルダウンメニューから「**ja-JP.json**」を選択します。
   * 「**選択翻訳データをダウンロード**」ボタンを押すと、公式リポジトリから最新の安定版が適用されます。  


2. **非公式リポジトリからダウンロード（先行版）**  
翻訳作業中の最新データや、未承認の修正をいち早く反映したい場合に使用します。
   * 「**作業場の最新翻訳データをダウンロード**」ボタンを押すと、開発中の最新翻訳データが直接ダウンロードされます。

---

## ⚠️ 仕様

### 🧠 文字化けのような表示について
プレイ中に文章へ `＆` や `＠` などの記号が混ざり、読みにくくなる現象が発生することがありますが、これは**ゲームの正常な仕様**です。

* **原因**: ゲーム内パラメータ **"Brain Health"（脳機能）** の低下
* 翻訳ミスやプラグインの不具合ではありません。ブレイングロウを摂取して回復してください。

***

## 🌐 翻訳コミュニティについて

この有志翻訳は、Discordの翻訳コミュニティにて制作されました。  
フィードバックや日本語化ツールに対するご意見、今後の翻訳アップデートに向けたご協力など、どなたでも大歓迎です。

👉 **[翻訳コミュニティ（Discord）はこちら！](https://discord.com/channels/955738554129063947/1445554981150261359)**  

### 🛠️管理者
* **marui-neko** [GitHub Profile](https://github.com/marui-neko)


### 🤝 翻訳・テストプレイ協力者
本プロジェクトは、以下の有志メンバーの皆様の多大なるご協力によって制作されています。心より感謝申し上げます！
* **RicecakeHuman**  [GitHub Profile](https://github.com/RicecakeHuman)
* **huwahuwa**
* **NEꞰ0**
* **spidragon**

***

## 📜 ライセンス・クレジット

<details><summary>ライセンス情報・使用フォント（クリックで展開）</summary>

### 🛠️ 日本語化パックに同梱しているツール
日本語化環境を構築するために、以下の3つを使用・同梱しています。
1. **BepInEx (x64版)**: UnityゲームにModを導入するための必須前提ツール。👉 [GitHub](https://github.com/BepInEx/BepInEx/releases)
2. **XUnity.ResourceRedirector-BepInEx**: フォントの読み込みを補助するために必要。👉 [GitHub](https://github.com/bbepis/XUnity.AutoTranslator/releases)
3. **CUFontPatcher**: フォントを個別に指定・調整し自動改行を追加する専用プラグイン。👉 [GitHub](https://github.com/marui-neko/CUFontPatcher/tree/main)
4. **CUTranslateSupporter**: 自動で日本語訳をダウンロード、適応、及び翻訳支援を行うツール。 👉 [GitHub](https://github.com/marui-neko/CUTranslateSupporter)
5. **CUImageReplacer**: ゲーム内の画像を置き換えるプラグイン。

### ライセンス
本パッケージには、導入作業を簡略化する目的で「BepInEx」を同梱しています。
BepInExは、GNU Lesser General Public License v2.1 (LGPL-2.1) の下でオープンソースとして提供されています。
* 詳しくは同梱の LICENSE.txt をご確認ください。
* ソースコード：[https://github.com/BepInEx/BepInEx](https://github.com/BepInEx/BepInEx)

### 使用フォント
本MODでは以下のフォントをアセットバンドル化して使用しています。
* **yuzupenkai_u_2019**: [配布元](https://black-yuzunyan.lolipop.jp/fonts-yuzu-pen-kai)
* **bestten_2018** (ベストテンFONT): [配布元](https://flopdesign.booth.pm/items/2747965)
* **dotgothic16**: [配布元](https://fonts.google.com/specimen/DotGothic16)
* **アームド・レモン**: [配布元](https://www.vector.co.jp/soft/data/writing/se334877.html)
* **適当ポエム**: [配布元](https://booth.pm/ja/items/4806814)

</details>

***
