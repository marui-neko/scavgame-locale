# Casualties Unknown (Scav Prototype) 日本語化

このリポジトリは、Casualties Unknown (Scav Prototype) の日本語翻訳ファイルを公開・配布するための場所です。

> [!WARNING]
> **注意：非公式のModツールです。導入はすべて自己責任で行ってください！**

**翻訳ファイル:**  
👉 [ja-JP.json](https://raw.githubusercontent.com/marui-neko/scavgame-locale/refs/heads/japanese-translation/ja-JP.json)  
（※リンク先で右クリックして 「名前を付けて保存」 を選択してください）

## ⚠️ 注意！ ⚠️

リンクを右クリックして「名前をつけてリンク先を保存」を選択すると、拡張子が `.txt` に変わってしまいます。  
**必ずリンク先に飛んでから**、右クリックして 「名前を付けて保存」 を選択してください。

***

## 🛠️ 導入に必要なもの

日本語化環境を構築するために、以下の3つを使用しました。  
必要ファイルを同梱した日本語化セットを用意しているため、個別にダウンロードする必要はありません。


1. **BepInEx (x64版)**  
   UnityゲームにModを導入するための必須前提ツール。  
   👉 [Releases · BepInEx/BepInEx (GitHub)](https://github.com/BepInEx/BepInEx/releases)

2. **XUnity.ResourceRedirector-BepInEx**  
   フォントの読み込みを補助する「XUnity.ResourceRedirector」を使うために必要。  
   👉 [Releases · bbepis/XUnity.AutoTranslator (GitHub)](https://github.com/bbepis/XUnity.AutoTranslator/releases)

3. **CUFontPatcher**  
   ゲーム内の様々なフォントを個別に指定・調整し、没入感を高めるための専用プラグイン。  
   👉 [Releases · bbepis/XUnity.AutoTranslator (GitHub)](https://github.com/marui-neko/CUFontPatcher/tree/main)

## ⚠️ 最初に確認！ ⚠️

ゲームのディレクトリ（保存場所）のパスに「日本語」が含まれているとBepInExが起動しないため、日本語化ツールが動作しません。

```text
NG： C:\新規ファイル\Game
推奨： C:\New_File\Game
```

必ず**英数字のみのパス**に配置してください。

***

## 📥 導入手順

1. 必要ファイルを同梱した[CU日本語化パック](https://mega.nz/file/u19wUCDQ#eWCWK0JQqwKsFnkWWy04v0HUcGmxRDGYi2Tz7fbD2Ic) をダウンロード。
2. 解凍した中身すべてを、ゲームの実行ファイル（`CasualtiesUnknown.exe`）と同じフォルダに配置。
3. ダウンロードした `ja-JP.json` を以下のフォルダに配置。

   配置場所： `CasualtiesUnknown_Data\Lang`

***

## 🔠 CUFontPatcherについて

* **CUFontPatcherの構成は以下のとおりです。**

   ```text
   CasualtiesUnknown/
   └── BepInEx/
        └── plugins/
             └── CUFontPatcher/
                  ├── CUFontPatcher.dll    ← 本ツール
                  ├── fontmap.txt          ← フォント設定ファイル
                  ├── dotgothic16_u2018    ← 使用するフォント1
                  └── (その他のフォント)   ← 使用するフォント2...
   ```

* **`fontmap.txt` の設定について**  
  フォントをカスタマイズしたい場合、このテキストファイルを編集することで、フォントの大きさや間隔、アウトラインを調整できます。詳しくはファイル内のコメントを参照してください。

***

## ⚙️ ゲーム内での言語設定

1. すべてのファイルの配置が終わったら、`CasualtiesUnknown.exe` からゲームを起動。
2. タイトル画面右上の言語選択メニューから **「日本語」** を選択。

***

## ⚠️ 既知の不具合・仕様

### 🧠 文字化けのような表示について

プレイ中に文章へ `＆` や `＠` などの記号が混ざり、読みにくくなる現象が発生することがありますが、これは**ゲームの正常な仕様**です。

* **原因**: ゲーム内パラメータ **"Brain Health"（脳機能）** の低下
* 翻訳ミスやプラグインの不具合ではありません。ブレイングロウをガブガブ飲んで回復してください。

***

## 📜 ライセンス・クレジット

### ライセンス

本パッケージには、導入作業を簡略化する目的で「BepInEx」を同梱しています。


BepInExは、GNU Lesser General Public License v2.1 (LGPL-2.1) の下でオープンソースとして提供されています。


・BepInExのライセンス全文については、同梱の LICENSE.txt をご確認ください。  
・BepInExのソースコードは、以下の公式リポジトリより入手可能です。


  [  https://github.com/BepInEx/BepInEx](https://github.com/BepInEx/BepInEx)

### フォント

本MODでは以下のフォントをアセットバンドル化して使用しています。

**sitest**  
[https://booth.pm/ja/items/6218691](https://booth.pm/ja/items/6218691)

**bestten_2018**  
フォント：ベストテンFONT  
フリーダウンロード：[https://flopdesign.booth.pm/items/2747965](https://flopdesign.booth.pm/items/2747965)

**dotgothic16**  
[https://fonts.google.com/specimen/DotGothic16](https://fonts.google.com/specimen/DotGothic16)

**musin**  
[https://modi.jpn.org/font_mushin.php](https://modi.jpn.org/font_mushin.php)

一部のフォントアセットは下記リンクより入手させていただきました。  
[https://note.com/allgames_kari/n/n627af62e595f](https://note.com/allgames_kari/n/n627af62e595f)  
[https://ux.getuploader.com/XAT_Alternative_fonts/](https://ux.getuploader.com/XAT_Alternative_fonts/)
