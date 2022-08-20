# Takuro Inoue Resume

[![textlint](https://img.shields.io/github/workflow/status/kawamataryo/resume/lint%20text?label=textlint&logo=github&color=yellow)](https://github.com/kawamataryo/resume/actions?query=workflow%3A%22lint+text%22)
[![build pdf](https://img.shields.io/github/workflow/status/kawamataryo/resume/build-pdf?label=build%20pdf&logo=github)](https://github.com/kawamataryo/resume/actions?query=workflow%3A%22build+pdf%22)
[![create issue](https://img.shields.io/github/workflow/status/kawamataryo/resume/create%20issue?label=create%20issue&logo=github&color=orange)](https://github.com/kawamataryo/resume/actions?query=workflow%3A%22create+issue%22)
[![release date](https://img.shields.io/github/release-date/kawamataryo/resume?color=blue&logo=github)](https://github.com/kawamataryo/resume/releases)

[ English | [日本語](https://github.com/takuro-inoue1913/resume/blob/master/README.ja.md) ]

## Data
- [GitHub Pages](https://takuro-inoue1913.github.io/resume/)  
  - This is a job resume that is available on the web. The content is the same as that of the CV README.md.
- [PDF](https://github.com/takuro-inoue1913/resume/releases)  
  - You can download the latest version of the PDF here.
- [File](https://github.com/takuro-inoue1913/resume/blob/master/docs/README.md)  
  - README.md that describes your work history.

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

### 🛠 Create release

When you push with a `v**` tag, GitHub Actions will run the build, generate the PDF, create a Release, and register the PDF to Assets.

```
$ git commit -m "add job"
$ git tag v1.0
$ git push origin --tags
```

### 📆 Remind update

Automatically generate issues every three months with GitHub Actions Schedules triggers to prompt you to update your resume.

To change the duration or stop the job, edit `.github/workflows/create-issue.yml`.  
To change the issue contents, edit `.github/ISSUE_TEMPLATE.md`.
