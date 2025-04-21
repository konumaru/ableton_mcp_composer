# Ableton Composer プロジェクト - GitHub Copilot 指示

このリポジトリは Ableton Live を使用した作曲プロジェクトのコンセプト管理のためのものです。GitHub Copilot は以下の指示に従ってサポートしてください。

## リポジトリの目的

このリポジトリは以下を管理するためのものです：

- 作曲のアイデアとコンセプトの体系的な管理
- 制作中の曲の進捗状況の追跡
- 参考音源や影響を受けた作品の情報記録
- 使用した音色、サンプル、テクニックのドキュメント化
- 作曲プロセスの学びを記録する

## コード補完の方針

1. **新規曲プロジェクト作成時**:
   - `templates/` ディエクトリ内のテンプレートに従った構造とファイル作成を提案する
   - 必要なMDファイル（concept.md, notes.md, references.md）の基本構造を提供する

2. **マークダウン編集時**:
   - 既存の構造や書式を尊重する
   - 技術的な説明が必要な場合は、Ableton Liveの機能や設定に関する詳細を提案する
   - リスト項目や表形式のデータ入力をサポートする

3. **音楽理論関連**:
   - コード進行、調性、リズムパターンなどの音楽理論に基づくサジェストを行う
   - ジャンルに適したBPM、キー、構成などの一般的なパラメータを提案する

## ファイル/ディレクトリ構造

```shell
├── README.md                # プロジェクト概要
├── projects/                # 個別の曲プロジェクト
│   └── <track_name>/        # 各曲のフォルダ (concept.md, notes.md, references.md など)
├── samples/                 # サンプル管理（drums, synths, vocals など）
├── techniques/              # テクニック関連ドキュメント
├── inspirations/            # インスピレーション資料
└── templates/               # プロジェクトテンプレート
```

## 曲プロジェクトの標準構成

各曲プロジェクトフォルダ（`projects/<track_name>/`）には、以下のファイルを含みます：

- `concept.md` - コンセプト、ムード、テーマ
- `notes.md` - 制作プロセスのノート
- `references.md` - 参考音源、影響を受けた作品
- `project_files/` - Abletonプロジェクトファイル（gitignoreに追加）

## テンプレート活用

新しい曲プロジェクト作成時には、`templates/` にあるテンプレートファイルを使用してください:

1. `concept_template.md` - 曲のコンセプトテンプレート
2. `project_structure.md` - プロジェクト構造ガイドライン

## 特定の注意点

- 大きなオーディオファイルやAbletonプロジェクトファイルはGitで管理しない方針です
- テンプレートの内容を尊重しつつ、プロジェクトごとに必要なカスタマイズを提案してください
- 曲のジャンルやスタイルに合わせた適切なアドバイスを提供してください
- アイデアを整理・分類するためのタグやカテゴリシステムの利用を推奨してください

## テンプレート活用の例

新しい曲プロジェクトを作成する場合:

```shell
# コマンド例
mkdir -p projects/new_track_name
cp templates/concept_template.md projects/new_track_name/concept.md
touch projects/new_track_name/notes.md
touch projects/new_track_name/references.md
mkdir projects/new_track_name/project_files
```

その後、`concept.md`ファイルを編集して曲の詳細情報を入力します。
