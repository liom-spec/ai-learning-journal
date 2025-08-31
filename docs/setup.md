# 環境セットアップ

このプロジェクトをローカル環境で動作させるためのセットアップ手順を説明します。

## 必要要件

- Miniconda（Python環境管理用）
- Git（未インストールの場合は以下参照）
- Visual Studio Code（VS Code、未インストールの場合は以下参照）

## セットアップ手順

### 1. Minicondaのインストール

Minicondaは軽量なPythonディストリビューションで、仮想環境の管理に最適です。

- [Miniconda公式サイト](https://docs.conda.io/en/latest/miniconda.html)から、OSに対応したインストーラーをダウンロードしてインストールしてください。

### 2. Gitのインストール

Gitが未インストールの場合は、以下からインストールしてください。

- [Git公式サイト](https://git-scm.com/downloads)

#### Git未導入環境でのリポジトリ取得

Gitコマンドが使えない場合は、GitHubリポジトリページから「Code」→「Download ZIP」でソースコードをダウンロードし、任意のフォルダに展開してください。

### 3. Visual Studio Code（VS Code）のインストールと連携

VS Codeが未インストールの場合は、以下からダウンロードしてください。

- [VS Code公式サイト](https://code.visualstudio.com/)

#### VS Code拡張機能

- Python Extension（ms-python.python）
- Jupyter Extension（ms-toolsai.jupyter）

#### リポジトリのクローンまたはフォルダ展開後

VS Codeの「ファイル」→「フォルダーを開く」からプロジェクトフォルダを開いてください。  
VS Codeは仮想環境（condaなど）を自動検出し、インタープリタとして選択できます。

### 4. リポジトリのクローン（Gitインストール済の場合）

以下のコマンドをコピーして実行してください：

```sh
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 5. 仮想環境の作成とアクティベート

`environment.yml` が存在しない場合は、以下のように手動で作成できます（必要なパッケージ例を記載してください）。

仮想環境の作成とアクティベートには以下のコマンドを使用します：

```sh
conda env create --name your-env-name --file environment.yml
conda activate your-env-name
```

## よくある問題

- MinicondaやGitのバージョンを確認してください。
- `environment.yml`の設定ミス: 必要な項目が記載されているか確認してください。
- Gitが使えない場合: ZIPダウンロード→展開→VS Codeで開く手順を利用してください。

## その他

詳細は [公式ドキュメント](https://example.com) を参照してください。
