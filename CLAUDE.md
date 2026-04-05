# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## リポジトリの目的

Padflux（ブラウザで動く音楽ツール）のブランド資産・コンテンツ・SNS情報を管理するドキュメントリポジトリ。コードは含まない。

## ディレクトリの役割

- `brand/` — ブランドの軸となる定義（コンセプト・トーン）。変更は慎重に。
- `note/` — noteへの投稿コンテンツ。`profile.md` はクリエイターページの原稿、`articles/` に記事原稿を連番管理。
- `social/` — 各SNSのアカウント情報。

## コンテンツ作成ルール

### トーン&マナー（`brand/voice.md` が正）

- です・ます調ベース
- 断定・煽り表現、架空のデータ、上から目線は禁止
- 短文と長文を交互に組み合わせてリズムを作る

### 記事ファイルの命名規則

```
note/articles/NNN_slug.md   # 例: 002_drum-launch.md
```

連番は3桁ゼロ埋め。スラッグはケバブケース（英数字・ハイフンのみ）。

### ファイルを開く場合

```bash
open -a CotEditor <ファイルパス>
```

## GitHub運用

- ブランチ：`main` のみ（ドキュメントリポジトリのため）
- コミットメッセージ：Conventional Commits形式
  - 記事追加 → `feat: note記事NNN「タイトル」を追加`
  - 情報更新 → `fix:` または `docs:`
  - ブランド定義変更 → `refactor:`
