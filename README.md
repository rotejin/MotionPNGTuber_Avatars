# MotionPNGTuber Avatars / アバター素材集

[MotionPNGTuber Player](https://github.com/rotejin/MotionPNGTuber_Player) で使用できるアバター素材集です。

> **Note**: このリポジトリは日本語で記載されています。

## ダウンロード方法

### 方法1: ZIPダウンロード（推奨）

1. 本リポジトリの **[Code] > [Download ZIP]** をクリック
2. ZIPを展開し、使いたいアバターのフォルダを取り出す
3. [MotionPNGTuber Player](https://github.com/rotejin/MotionPNGTuber_Player) の `assets/` フォルダに配置

### 方法2: Git Clone

```bash
git clone https://github.com/rotejin/MotionPNGTuber_Avatars.git
```

clone後、使いたいアバターのフォルダを [MotionPNGTuber Player](https://github.com/rotejin/MotionPNGTuber_Player) の `assets/` フォルダに配置してください。

## アバター一覧

| アバター名 | プレビュー | 作者 | ライセンス |
|-----------|-----------|------|-----------|
| (準備中) | - | - | - |

> 各アバターの詳細（作者、ライセンス、利用条件）は、アバターフォルダ内の `README.md` を参照してください。

## アセット構成

各アバターは以下の構成になっています：

```
avatar_name/
├── README.md                # 作者・ライセンス・利用条件（必須）
├── preview.png              # プレビュー画像（推奨）
├── *_mouthless_h264.mp4     # 口消し済み動画（H.264, CFR）
├── mouth_track.json         # トラッキングデータ
└── mouth/
    ├── closed.png           # 口閉じ（必須）
    ├── open.png             # 口開き（必須）
    ├── half.png             # 半開き
    ├── e.png                # 「え」の口
    └── u.png                # 「う」の口
```

## 自作アバターの作成方法

1. [MotionPNGTuber](https://github.com/rotejin/MotionPNGTuber)（Python版）でループ動画をキャリブレーション
2. 口消し動画と `mouth_track.json` を生成
3. 口スプライト（PNG）を用意
4. 上記の構成でフォルダにまとめる

詳細は [MotionPNGTuber のREADME](https://github.com/rotejin/MotionPNGTuber) を参照してください。

## ライセンス

### アバター素材について

**各アバターのライセンスは、アバターフォルダ内の `README.md` に記載されています。**

- 利用前に必ず各アバターの利用条件を確認してください
- 作者によってクレジット表記、改変、商用利用などの条件が異なります

### リポジトリ構成ファイルについて

このREADME.md およびリポジトリ構成に関するファイルは [MIT License](LICENSE) です。

> **重要**: ルートの `LICENSE` ファイル（MIT）はリポジトリ構成・ドキュメントにのみ適用され、アバター素材（動画・画像・トラッキングデータ）には適用されません。

## 関連リンク

- [MotionPNGTuber](https://github.com/rotejin/MotionPNGTuber) - Python版（動画解析・キャリブレーション用）
- [MotionPNGTuber Player](https://github.com/rotejin/MotionPNGTuber_Player) - ブラウザ版プレイヤー
