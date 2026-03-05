
***

# Casualties Unknown (Scav Prototype) 日本語化

このリポジトリは、Casualties Unknown (Scav Prototype) の日本語翻訳ファイルを公開・配布するための場所です。

> [!WARNING]
> **注意：非公式のModツールです。導入はすべて自己責任で行ってください！**

***

## 📥 導入手順

### ⚠️ ゲームの保存場所に注意！
ゲームのフォルダパスに「日本語」が含まれていると、日本語化ツールが動作しません。
* ❌ NG： `C:\新規ファイル\CasualtiesUnknow`
* ⭕ 推奨： `C:\New_File\CasualtiesUnknow`


必ず**英数字のみのパス**に配置してください。


***


### 📥 導入ステップ

1. [**CU日本語化パック**](https://mega.nz/file/3p1WEapD#UnUypbcGev4Pgf1JelWCgH-uwuaX1Mi6rtdo8DDnY7Y)をダウンロード  
   必要ファイルがすべて入っています。ダウンロードして解凍してください。

2. **ゲームフォルダに配置**  
   解凍した中身すべてを、ゲームの実行ファイル（`CasualtiesUnknown.exe`）と同じフォルダに配置します。

3. **翻訳ファイルをダウンロード＆配置**  
   👉 **[ja-JP.json](https://raw.githubusercontent.com/marui-neko/scavgame-locale/refs/heads/japanese-translation/ja-JP.json)** 
   （※リンク先で右クリックして 「名前を付けて保存」）  

> [!WARNING]
   >**翻訳ファイルの保存方法に注意！**  
> **必ずリンク先に飛んでから**、右クリックして 「名前を付けて保存」 を選択してください。  
   >リンクを右クリックして「名前をつけてリンク先を保存」を選択すると、拡張子が `.txt` に変わってしまいます。  

   
   ダウンロードした `ja-JP.json` を以下のフォルダに配置します。
   * 配置場所： `CasualtiesUnknown_Data\Lang`

4. **ゲーム起動＆設定**
   すべての配置が終わったら、`CasualtiesUnknown.exe` からゲームを起動  
   タイトル画面右上の言語選択メニューから **「日本語」** を選択すれば完了です。

***

## ⚙️ さらにカスタマイズしたい人へ

### オプション設定：自動改行の無効化
デフォルトでは自動改行が有効になっています。無効にしたい場合は、以下の手順で設定を変更してください。

1. `BepInEx\plugins\CUFontPatcher\fontmap.txt` をメモ帳などで開く。
2. `enableautowrap=` の値を `False` に書き換えて保存する。

※設定変更は、保存後にゲーム内テキストを再表示すると反映されます。ゲーム内の書き置きなどを見ながら調整するのがおすすめです。

## ⚠️ 既知の不具合・仕様

### 🧠 文字化けのような表示について
プレイ中に文章へ `＆` や `＠` などの記号が混ざり、読みにくくなる現象が発生することがありますが、これは**ゲームの正常な仕様**です。

* **原因**: ゲーム内パラメータ **"Brain Health"（脳機能）** の低下
* 翻訳ミスやプラグインの不具合ではありません。ブレイングロウをガブガブ飲んで回復してください。

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

***

## 📜 ライセンス・クレジット

<details><summary>ライセンス情報・使用フォント（クリックで展開）</summary>

### 🛠️ 日本語化パックに同梱しているツール
日本語化環境を構築するために、以下の3つを使用・同梱しています。
1. **BepInEx (x64版)**: UnityゲームにModを導入するための必須前提ツール。👉 [GitHub](https://github.com/BepInEx/BepInEx/releases)
2. **XUnity.ResourceRedirector-BepInEx**: フォントの読み込みを補助するために必要。👉 [GitHub](https://github.com/bbepis/XUnity.AutoTranslator/releases)
3. **CUFontPatcher**: フォントを個別に指定・調整し自動改行を追加する専用プラグイン。👉 [GitHub](https://github.com/marui-neko/CUFontPatcher/tree/main)

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
