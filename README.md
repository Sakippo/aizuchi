# Aizuchi — 規約・プライバシーポリシー

Aizuchi アプリのプライバシーポリシーと利用規約を公開するための静的サイトです。

## 構成

| ファイル | 内容 |
|---|---|
| `index.html` | トップページ（各ページへのリンク） |
| `privacy-policy.html` | プライバシーポリシー |
| `terms.html` | 利用規約 |
| `style.css` | 共通スタイル |

## GitHub Pages で公開する手順

1. GitHub で新しい **public** リポジトリを作成する（例：`aizuchi`）。
2. このフォルダの中身をそのリポジトリにプッシュする。
   ```sh
   cd aizuchi
   git init
   git add .
   git commit -m "Add privacy policy and terms of service"
   git branch -M main
   git remote add origin https://github.com/<あなたのユーザー名>/aizuchi.git
   git push -u origin main
   ```
3. リポジトリの **Settings → Pages** を開く。
4. **Build and deployment → Source** で `Deploy from a branch` を選び、Branch を `main` / `/ (root)` にして Save。
5. 数分後、以下の URL で公開される。
   - トップ：`https://<あなたのユーザー名>.github.io/aizuchi/`
   - プライバシーポリシー：`https://<あなたのユーザー名>.github.io/aizuchi/privacy-policy.html`
   - 利用規約：`https://<あなたのユーザー名>.github.io/aizuchi/terms.html`

## 公開後にやること

- 上記 URL をアプリ側の `AppLinks`（`synvoice/utils/UI/AppConstants.swift`）に設定する。
- App Store Connect の「App のプライバシー」および「プライバシーポリシー URL」に上記 URL を登録する。

## 更新方法

内容を変更したら、ファイルの「最終更新日」を更新してプッシュし直すだけで反映されます。
