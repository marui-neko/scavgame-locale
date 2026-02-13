# 🇯🇵 Casualties Unknown (Scav Prototype) 日本語化

このリポジトリは、**Casualties Unknown (Scav Prototype)** の日本語翻訳ファイルを公開するためのフォークです。

**翻訳ファイル:**  
👉 [JA.json](https://github.com/marui-neko/scavgame-locale/blob/main/JA.json)

---

## 🛠️ 導入に必要なもの

1.  **XUnity.AutoTranslator**  
    Unity製ゲームの自動翻訳・文字置換ツール。
2.  **日本語フォント**  
    ゲーム内で日本語を正しく表示するために必須。
3.  **JA.json**  
    本リポジトリで配布している翻訳データ。

---

## 📥 導入手順

### 1. 翻訳ファイルの配置
ダウンロードした `JA.json` を以下のフォルダに配置。
`CasualtiesUnknown\CasualtiesUnknown_Data\Lang`

### 2. フォントの準備
テスト環境では **Gothic-regular_u2019** を使用

*   **入手先**: [XAT_Alternative_fonts (uploader.com)](https://ux.getuploader.com/XAT_Alternative_fonts/)
*   **配置場所**: ゲームの実行ファイル（`CasualtiesUnknown.exe`）と同じフォルダに配置

### 3. Config.ini の設定
XUnity.AutoTranslatorを導入後、生成される `Config.ini`（AutoTranslatorフォルダ内）をテキストエディタで開き、`[Behaviour]` セクションを以下のように編集

```ini
[Behaviour]
FallbackFontTextMeshPro=Gothic-regular_u2019

```

> [!IMPORTANT]
> **設定の注意点**
> *   **推奨**: `FallbackFontTextMeshPro` ライフポッド内の書き置きなどは別フォントが使われているため、数字などが入ると表示が乱れるが大体いい感じ
> *   **非推奨**: `OverrideFontTextMeshPro`　文字が全体的に濁る

### 4. ゲーム内設定の変更
タイトル画面右上から「日本語」を選択

---

## ⚠️ 既知の不具合・仕様について

### 🐛 表示の乱れ
*   **タイトルのあらすじ表示が崩れる**
    *   現状、解決策が見つかっておりません。

### 🧠 文字化けのような表示について
プレイ中に文章へ `＆` や `＠` などの記号が混ざり、読みにくくなる現象が発生することがありますが、これは**ゲームの仕様**です。

*   **原因**: ゲーム内パラメータ **"Brain Health"（脳機能）** の低下
*   翻訳ミスや不具合ではありませんので、ブレイングロウをガブガブしてください。
