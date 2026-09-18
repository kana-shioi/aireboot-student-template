# AI Re:Commit 受講者用テンプレート

このリポジトリは「AI Re:Commit」の受講用テンプレートです。
GitHub Codespaces を起動すると、**Claude Code が自動でインストール済み**の状態で開発を始められます。

## セットアップの流れ

1. このリポジトリのページ右上にある緑色の **「Use this template」** ボタンから、
   **自分の GitHub リポジトリを作成**します。
   このとき、公開範囲は必ず **Private(非公開)** を選んでください。
2. 作成した**自分のリポジトリ**を開き、**「Code」→「Codespaces」→「Create codespace on main」** で
   Codespace を起動します。
3. 起動後、Claude Code の自動インストールが始まります。
   ターミナルに次のメッセージが表示されるまで**待ってください**。

   ```
   ✅ Claude Code の準備が完了しました。ターミナルで claude と入力して開始できます。
   ```

   > ⚠️ このメッセージが出る前に `claude` を実行すると `command not found` になります。
   > インストール完了まで実行を待ってください。

## 動作確認

セットアップ完了後、ターミナルで次のコマンドを実行し、バージョンが表示されれば成功です。

```bash
claude --version
```

## サインイン

`claude` を初めて起動すると、Claude アカウントでのサインインが求められます。
**サインインの詳しい手順(認証コードのコピペ含む)は、講座の Day0 画面**を参照してください。

## トラブルシューティング

### `claude: command not found` と表示される

1. まずはインストール完了メッセージが出るまで待てているか確認してください。
2. それでも表示される場合は、ターミナルで手動インストールを実行します。

   ```bash
   npm install -g @anthropic-ai/claude-code
   ```

3. 上記でも解決しない場合は、Codespace を**リビルド**してください。
   コマンドパレット(`F1` または `Ctrl/Cmd + Shift + P`)を開き、
   **「Codespaces: Rebuild Container」** を実行します。
