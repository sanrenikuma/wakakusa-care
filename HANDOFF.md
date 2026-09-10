# HANDOFF

## 更新情報

- 更新日時: 2026-09-10 Asia/Tokyo
- 更新者: Cursor
- 現在の目的: サービス・採用の挿絵を新しい水彩に差し替えたホームページを、確認済みの事実だけを保ったまま公開する。

## 現在の状態

- ブランチ: `main`
- HEAD / upstream: `main` は `origin/main` と一致させる。hero は未変更。サイト本体の直前公開は `1caecd9`。
- 作業ツリー: 変換元 PNG は未追跡のまま残る。ページは参照しない。`.DS_Store` は対象外。
- GitHub: `https://github.com/sanrenikuma/wakakusa-care`
- 公開先: Vercel。`https://wakakusa-care.com/` と `https://wakakusa-care.vercel.app/`
- 構成: `index.html`、画像（JPEG / WebP）、`thanks.html`、`favicon.svg`。フォーム送信先は従来の Formspree のまま。

## 直近で完了したこと

- ChatGPT生成の水彩6枚を、既存ファイル名の JPEG / WebP に変換して差し替えた。hero は残した。
- `index.html` の画像サイズと alt を新しい絵に合わせた。

## 検証済み

- `git diff --check` — 成功。2026-09-10。
- 内部アンカー、ローカル画像ファイルの存在、画像alt、JSON-LD — 成功。2026-09-10。この差し替え後。
- 未実施: 差し替え後の本番目視。実機iPhone、キーボード操作、文字200%、フォーム実送信。事業所側の最終確認。

## 次に行うこと

1. push 後に本番をスマホ幅・PC幅で目視し、サービスカードと採用写真を確認する。
2. 事業所側に求人条件・対応エリア・フォーム受信と同意文面の最終確認を依頼する。

## 判断待ち・禁止事項

- 判断待ち: 求人の給与・勤務条件、対応エリア、Formspree完了後の運用。
- 禁止事項: 明示承認なしに commit、push、deploy、フォーム送信、送信先や公開ドメインの変更を行わない。
- 禁止事項: 秘密情報をリポジトリやこのファイルへ書かない。`.DS_Store` と PNG 原画は自動追加しない。

## 関連資料

- 恒久ルール: `AGENTS.md`
- 設計文書: なし
- 詳細な旧引き継ぎ記録: なし
