# FF14 Toolbox — Mitigation Table

このリポジトリは Final Fantasy XIV 向けの軽減参照表と関連ツールを収めるためのリポジトリです。  
ブラウザで開くだけで使える静的 HTML を中心に、今後ツールを追加していく想定で構成しています。

---

## 概要

**ff14-mitigation-table.html** をはじめ、将来的に複数のツールやドキュメントを追加していきます。  
各ツールは独立した HTML ファイルとして配置し、GitHub Pages で公開することを想定しています。

---

## リンク

- **公開ページ**: https://hy11-hiro.github.io/ff14-toolbox/ff14-mitigation-table.html  
- **リポジトリ**: https://github.com/hy11-hiro/ff14-toolbox

---

## リポジトリ構成例

- `docs/` — GitHub Pages 公開用ファイル（`ff14-mitigation-table.html` 等）  
- `tools/` — 将来のスクリプトやユーティリティ（例: `mitigation/`）  
- `assets/` — 画像・CSS・JS 等の共有リソース  
- `README.md` — このファイル  
- `LICENSE` — リポジトリ全体のライセンス  
- `CHANGELOG.md` — 変更履歴

---

## 追加手順（簡潔）

1. **ファイルを作成**  
   - 新しいツールは `docs/` または `tools/` に配置。静的ページは `docs/` 推奨。  
2. **ブランチを作る**  
   - `git checkout -b feature/<short-description>` 例: `feature/add-mitigation-table`  
3. **コミット**  
   - コミットメッセージ例: `feat: add ff14-mitigation-table.html`  
4. **プルリクエストを作成**  
   - PR タイトル例: `Add ff14 mitigation table`  
   - 変更点を簡潔に記載し、スクリーンショットや確認手順を添える  
5. **レビューとマージ**  
   - レビュー後 `main` にマージ。緊急のホットフィックスは `hotfix/` ブランチを使用。

---

## 貢献ルール

- **小さな修正**は `feature/` または `fix/` ブランチで作業して PR を送ってください。  
- **PR に含めるもの**: 変更の目的、影響範囲、確認手順（表示・印刷チェック等）。  
- **データ更新**はコミットメッセージに対応パッチと最終更新日を明記してください（例: `docs: update mitigation values for patch 6.x — 2026-01-16`）。  
- **命名規則**: ファイル名は英語小文字とハイフンで統一（例: `ff14-mitigation-table.html`）。  
- **資産管理**: 画像やフォントは `assets/` にまとめ、相対パスで参照してください。

---

## ライセンスと更新履歴

- **コード**: **MIT License** を推奨（`LICENSE` に記載）  
- **コンテンツ**: 再配布を許可する場合は **CC BY-SA 4.0** を推奨（ページ内に明記）  
- **CHANGELOG**: 重要な変更は `CHANGELOG.md` に記載。フォーマット例: `v1.0 — YYYY-MM-DD — 内容`。

---

## チェックリスト（ファイル追加時）

- [ ] `docs/` または `tools/` にファイルを配置した  
- [ ] `README.md` に該当ツールのリンクを追加した  
- [ ] コミットメッセージに要点（何を、どのパッチ向けか）を記載した  
- [ ] PR に確認手順（表示・印刷・モバイル）を記載した  
- [ ] `CHANGELOG.md` にエントリを追加した（必要時）  
- [ ] ライセンス表記をページ内に明記した

---

## 補足

- **公開方法**: `docs/` を GitHub Pages の公開ソースに設定すると簡単に公開できます。  
- **将来的な拡張**: JSON データを読み込む方式にすれば、データ更新を自動化しやすくなります。  
