# 井上拓郎の職務経歴書

[![textlint](https://img.shields.io/github/workflow/status/kawamataryo/resume/lint%20text?label=textlint&logo=github&color=yellow)](https://github.com/kawamataryo/resume/actions?query=workflow%3A%22lint+text%22)
[![build pdf](https://img.shields.io/github/workflow/status/kawamataryo/resume/build-pdf?label=build%20pdf&logo=github)](https://github.com/kawamataryo/resume/actions?query=workflow%3A%22build+pdf%22)
[![create issue](https://img.shields.io/github/workflow/status/kawamataryo/resume/create%20issue?label=create%20issue&logo=github&color=orange)](https://github.com/kawamataryo/resume/actions?query=workflow%3A%22create+issue%22)

[ [English](https://github.com/takuro-inoue1913/resume/blob/master/README.md) | 日本語 ]

## Data
- [GitHub Pages](https://takuro-inoue1913.github.io/resume/)  
  - Webで公開している職務経歴書です。内容は[職務経歴書README.md](https://github.com/takuro-inoue1913/resume/blob/master/docs/README.md)と同じです。
- [PDF](https://github.com/takuro-inoue1913/resume/releases)  
  - ここから最新バージョンのPDFをダウンロード出来ます。
- [File](https://github.com/takuro-inoue1913/resume/blob/master/docs/README.md)  
  - 職務経歴書を記載しているREADME.mdです。

## Features

### 

### ✨ Lint
```
$ yarn lint:fix
```

### 📝 Generate PDF
```
$ yarn build:pdf
```
出力されるPDFはCSSで任意のスタイルを設定可能です。pdf-configs/style.cssを編集してください。

### 🛠 Create release

v** tagをつけてpushするとGitHub Actionsでビルドが走り、PDFの生成、Releaseの作成、AssetsへPDFの登録が実行されます。

```
$ git commit -m "add job"
$ git tag v1.0
$ git push origin --tags
```

### 📆 Remind update

GitHub Actionsのschedule triggerで3ヶ月に1回、職務経歴書の内容更新を促すissueが自動生成されます。

期間を変更したり、ジョブを停止するには、 `.github/workflows/create-issue.yml` を編集してください。 
課題の内容を変更するには、`.github/ISSUE_TEMPLATE.md` を編集してください。
