# HANDOFF

## 更新情報

- 更新日時: 2026-09-10 Asia/Tokyo
- 更新者: Cursor
- 現在の目的: レビュー指摘を直したホームページを、確認済みの事実だけを保ったまま運用する。

## 現在の状態

- ブランチ: `main`
- HEAD / upstream: `1caecd9`。ローカルと `origin/main` は一致。
- 作業ツリー: サイト差分なし。`.DS_Store` は対象外。
- GitHub: `https://github.com/sanrenikuma/wakakusa-care`
- 公開先: Vercel。`https://wakakusa-care.com/` と `https://wakakusa-care.vercel.app/`
- 構成: `index.html`、画像（JPEG / WebP）、`thanks.html`、`favicon.svg`。フォーム送信先は従来の Formspree のまま。

## 直近で完了したこと

- `1caecd9 fix: 相談と採用の導線と読みやすさを直す` を `main` に commit し、`origin/main` へ push した。
- スマホ固定バー、採用からの種別着地、同意チェック、コントラスト、未確認の求人断定、画像圧縮を反映した。

## 検証済み

- `git diff --check` — 成功。2026-09-10。
- 内部アンカー、ローカル画像、画像alt、JSON-LD、電話・メール・住所・Formspree送信先 — 成功。2026-09-10。
- 本番HTMLに「利用相談をする」「採用情報を見る」「送信する」があること、`thanks.html` / `favicon.svg` / `hero.webp` の HTTP 200 — 成功。2026-09-10。両方の公開URLで確認。
- 未実施: 実機iPhone、キーボードだけの操作、文字200%、フォーム実送信、本番のスマホ・PC目視。

## 次に行うこと

1. 本番をスマホ幅・PC幅で目視し、ヘッダー、固定バー、採用カード、フォームを確認する。
2. 事業所側に求人条件・対応エリア・フォーム受信と同意文面の最終確認を依頼する。

## 判断待ち・禁止事項

- 判断待ち: 求人の給与・勤務条件、対応エリア、Formspree完了後の運用。
- 禁止事項: 明示承認なしに commit、push、deploy、フォーム送信、送信先や公開ドメインの変更を行わない。
- 禁止事項: 秘密情報をリポジトリやこのファイルへ書かない。`.DS_Store` は自動追加しない。

## 関連資料

- 恒久ルール: `AGENTS.md`
- 設計文書: なし
- 詳細な旧引き継ぎ記録: なし
