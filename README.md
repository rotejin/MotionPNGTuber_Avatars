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

## コントリビュート

アバターの追加は大歓迎です！Pull Requestをお待ちしています。

### 提出時のチェックリスト

アバターを提出する際は、以下を含めてください：

- [ ] **アバターフォルダ**（例: `my_avatar/`）
- [ ] **README.md**（必須）: 以下の情報を記載
  - 作者名
  - ライセンス（CC BY, CC BY-NC, 独自ライセンス等）
  - クレジット表記の要否
  - 改変・再配布の可否
  - 商用利用の可否
  - 連絡先（任意）
- [ ] **preview.png**（推奨）: プレビュー画像
- [ ] **動作確認済み**: MotionPNGTuber Player で正常に動作すること
- [ ] **必須ファイル**: `*_mouthless_h264.mp4`, `mouth_track.json`, `mouth/closed.png`, `mouth/open.png`

### アバターREADMEテンプレート

アバターフォルダ内の `README.md` は以下を参考にしてください：

```markdown
# アバター名

## 作者
- 名前: your_name
- 連絡先: (任意)

## ライセンス
CC BY 4.0 / CC BY-NC 4.0 / 独自ライセンス など

## 利用条件
- クレジット表記: 必要 / 不要
- 改変: 可 / 不可
- 再配布: 可 / 不可
- 商用利用: 可 / 不可

## 備考
(任意の説明)
```

## 関連リンク

- [MotionPNGTuber](https://github.com/rotejin/MotionPNGTuber) - Python版（動画解析・キャリブレーション用）
- [MotionPNGTuber Player](https://github.com/rotejin/MotionPNGTuber_Player) - ブラウザ版プレイヤー
