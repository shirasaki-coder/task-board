# CLAUDE.md

このファイルは、このリポジトリで Claude Code (claude.ai/code) が作業する際のガイドラインです。

## プロジェクト概要

**task-board** — タスクボードアプリ。

- 技術スタック: React（Vite）
- 機能: テキスト入力でのタスク追加、チェックボックスによる完了/未完了の切り替え、タスク削除、完了済みタスクのグレー表示

## Git 運用ルール

- **コードに変更を加えるたびに、コミットして GitHub にプッシュすること。** 作業を溜め込まず、変更単位ごとに commit → push を行う。
- コミットメッセージは変更内容が分かるように簡潔に書く。
- push 前に `git status` で意図しないファイル（secrets、ビルド成果物など）が含まれていないか確認する。
- force push や履歴を書き換える操作（`git reset --hard`、`git push --force` 等）はユーザーの明示的な許可なしに行わない。
- リモートリポジトリ（GitHub）が未設定の場合は、push の前にユーザーに remote の URL を確認する。

## コマンド

- `npm install` — 依存関係のインストール
- `npm run dev` — 開発サーバー起動
- `npm run build` — 本番ビルド
- `npm run lint` — oxlint による静的解析
