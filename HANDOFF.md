# HANDOFF

## 更新情報

- 更新日時: 2026-09-10 Asia/Tokyo
- 更新者: Cursor
- 現在の目的: 新しい水彩挿絵を入れたホームページを、確認済みの事実だけを保ったまま運用する。

## 現在の状態

- ブランチ: `main`
- HEAD / upstream: `main` は `origin/main` と一致。挿絵差し替えは `c22935b`。hero は未変更。
- 作業ツリー: サイト差分なし。PNG 原画と未使用の `volunteer.jpg` は削除済み。`.DS_Store` は対象外。
- GitHub: `https://github.com/sanrenikuma/wakakusa-care`
- 公開先: Vercel。`https://wakakusa-care.com/` と `https://wakakusa-care.vercel.app/`
- 構成: `index.html`、画像（JPEG / WebP）、`thanks.html`、`favicon.svg`。フォーム送信先は従来の Formspree のまま。

## 直近で完了したこと

- `c22935b feat: サービスと採用の挿絵を新しい水彩に差し替える` を push した。hero は残した。
- ユーザーが差し替え後の本番を確認し、問題なしとした（2026-09-10）。
- ページ未参照の PNG 原画6枚と、未使用の `volunteer.jpg` を削除した。差し替え前の JPEG/WebP は同名上書き済みで、別ファイルとしては残っていない。

## 検証済み

- `git diff --check` — 成功。2026-09-10（画像差し替え時）。
- 内部アンカー、ローカル画像ファイルの存在、画像alt、JSON-LD — 成功。2026-09-10。
- 差し替え後の本番目視 — 問題なし。2026-09-10。ユーザー確認。
- 未実施: 実機iPhone、キーボード操作、文字200%、フォーム実送信。事業所側の最終確認。

## 次に行うこと

1. 事業所側に求人条件・対応エリア・フォーム受信と同意文面の最終確認を依頼する。

## 判断待ち・禁止事項

- 判断待ち: 求人の給与・勤務条件、対応エリア、Formspree完了後の運用。
- 禁止事項: 明示承認なしに commit、push、deploy、フォーム送信、送信先や公開ドメインの変更を行わない。
- 禁止事項: 秘密情報をリポジトリやこのファイルへ書かない。`.DS_Store` は自動追加しない。

## 関連資料

- 恒久ルール: `AGENTS.md`
- 設計文書: なし
- 詳細な旧引き継ぎ記録: なし
