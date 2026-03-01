# VRM Pose Viewer

VRMキャラクターのポーズを編集・PNG出力できるWebビューアです。

## 機能

- VRMファイルの読み込み（ファイル選択 / ドラッグ&ドロップ）
- 1人 / 2人モード
- プリセットポーズ（立ち・座り・後傾・寄り添いなど）
- ボーン個別調整スライダー
- Pose JSON 読み込み / エクスポート
- PNG保存・クリップボードコピー（512〜1536px）

## デフォルトVRMの配置

`chara_a.vrm` / `chara_b.vrm` をこのディレクトリに置くと
URLパラメータで自動ロードできます。

```
# 1人
https://your-app.vercel.app/?vrm=chara_a.vrm

# 2人
https://your-app.vercel.app/?vrm_a=chara_a.vrm&vrm_b=chara_b.vrm
```

## デプロイ

GitHubにpush → Vercelでimport するだけ。

```bash
git init
git add .
git commit -m "initial"
# GitHub リポジトリを作成してpush
# Vercel で該当リポジトリをimport
```
