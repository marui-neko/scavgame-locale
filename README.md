# Casualties Unknown (Scav Prototype) 日本語化

このリポジトリは、Casualties Unknown (Scav Prototype) の日本語翻訳ファイルを公開・編集・配布するための場所です。

> [!WARNING]
> **注意：非公式ですので自己責任で導入してください！**

**翻訳ファイル:**  
👉 [ja-JP.json](https://github.com/marui-neko/scavgame-locale/blob/japanese-translation/ja-JP.json)

***

## 🛠️ 導入に必要なもの

1.  **XUnity.AutoTranslator -ReiPatcher-**  
    Unity製ゲームの自動翻訳・文字置換ツール
    [Releases · bbepis/XUnity.AutoTranslator (GitHub)](https://github.com/bbepis/XUnity.AutoTranslator/releases)
    
2.  **日本語フォント (AssetBundle)**  
    ゲーム内で日本語を正しく表示するために必須  
    推奨は本リポジトリで配布しているフォント
    
4.  **ja-JP.json**  
    本リポジトリで配布している翻訳データ

***

## 📥 導入手順

### 1. 自動翻訳ツールの準備
1.  [`XUnity.AutoTranslator-ReiPatcher`](https://github.com/bbepis/XUnity.AutoTranslator/releases) をダウンロード。
2.  解凍した中身（`SetupReiPatcherAndAutoTranslator.exe`）をゲームの実行ファイル（`CasualtiesUnknown.exe`）と同じフォルダに配置。
3.  `SetupReiPatcherAndAutoTranslator.exe` を起動。
4.  同フォルダに `ReiPatcher` フォルダが作成されているのを確認後、`CasualtiesUnknown (Patch and Run).exe` を実行してゲームを起動。起動後はゲームを終了させる。
4.  同フォルダに `AutoTranslator` フォルダが作成されているのを確認できたら導入は完了です。

> [!IMPORTANT]
> **パッチが当てられない**
> *   `CasualtiesUnknown (Patch and Run).exe`を実行してもゲームが起動できずパッチが当てられない症状が出ますが、これはwindows defenderのセキュリティが反応している可能性があります。（[Windows によって PC が保護されました]と出てくるやつ。）   
      その場合一度ゲームを起動することでパッチが当てられるようになります。

### 2. 翻訳ファイルの配置
ダウンロードした `ja-JP.json` を以下のフォルダに配置。
`CasualtiesUnknown\CasualtiesUnknown_Data\Lang`

### 3. フォントの準備
テスト環境では **dotgothic16_u2018** を使用。

*   **入手先**: [dotgothic16_u2018 のダウンロード](https://github.com/marui-neko/scavgame-locale/raw/refs/heads/japanese-translation/dotgothic16_u2018)
*   **配置場所**: ゲームの実行ファイル（`CasualtiesUnknown.exe`）と同じフォルダに配置。

### 4. Config.ini の設定
XUnity.AutoTranslator導入後に生成される `Config.ini`（`AutoTranslator`フォルダ内）をテキストエディタで開き、`[Behaviour]` セクションの中から `FallbackFontTextMeshPro=` を探し、以下のように編集。

```ini
[Behaviour]
~~
OverrideFontTextMeshPro=
FallbackFontTextMeshPro=dotgothic16_u2018
```

> [!IMPORTANT]
> **設定の注意点**
> *   **推奨**: `FallbackFontTextMeshPro` ライフポッド内の書き置きなどは別フォントが使われているため、数字などが入ると表示が乱れるが大体いい感じ。
> *   **非推奨**: `OverrideFontTextMeshPro`　文字が全体的に濁る。

### 5. パッチ＆ゲーム内設定の変更
1.  `CasualtiesUnknown (Patch and Run).exe` を実行してゲームを起動。
2.  タイトル画面右上から `日本語` を選択。

***

## ⚠️ 既知の不具合・仕様について

### 🐛 表示の乱れ
*   **タイトルのあらすじ表示が崩れる**
    *   現状、解決策が見つかっておりません。

### 🧠 文字化けのような表示について
プレイ中に文章へ `＆` や `＠` などの記号が混ざり、読みにくくなる現象が発生することがありますが、これは**ゲームの仕様**です。

*   **原因**: ゲーム内パラメータ **"Brain Health"（脳機能）** の低下
*   翻訳ミスや不具合ではありませんので、ブレイングロウをガブガブしてください。

***

## 📜 ライセンス・クレジット

### フォント
本MODでは以下のフォントをアセットバンドル化して使用しています。
*   **DotGothic16** (Licensed under SIL Open Font License 1.1)
    *   Original Author: Fontworks Inc.
    *   License: [https://scripts.sil.org/OFL](https://scripts.sil.org/OFL)
