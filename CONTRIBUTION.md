# 代码贡献指南
1. 非常欢迎和感谢对本项目发起Pull Request的同学，本项目代码风格为使用2个空格代表一个Tab，因此在提交代码时请注意一下，否则很容易在IDE格式化代码后与原代码产生大量diff，这样会给其他人阅读代码带来极大的困扰。为了便于设置，本项目引入editorconfig插件，请使用eclipse的同学在贡献代码前安装相关插件，IntelliJ IDEA新版本自带支持，如果没有可自行安装插件。
1. 本项目可以采用两种方式接受代码贡献：
  * 第一种就是基于[Git Flow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)开发流程，因此在发起Pull Request的时候请选择develop分支，详细步骤参考后文。
  * 另外一种贡献代码的方式就是加入SDK Developers开发组，前提是对自己的代码足够自信就可以申请加入，加入之后可以随时直接提交代码，但要注意对所做的修改或新增的代码进行单元测试，保证提交代码没有明显问题，具体加入方式，请咨询QQ群管理员。


### PR方式贡献代码步骤
* 在 GitHub 上 `fork` 到自己的仓库，如 `my_user/best-pay-sdk`，然后 `clone` 到本地，并设置用户信息。

```bash
$ git clone git@github.com:my_user/best-pay-sdk.git
$ cd best-pay-sdk
$ git config user.name "yourname"
$ git config user.email "your email"
```
* 修改代码后提交，并推送到自己的仓库。

```bash
$ #do some change on the content
$ git commit -am "Fix issue #1: change something"
$ git push
```
* 在 GitHub 网站上提交 Pull Request。
* 定期使用项目仓库内容更新自己仓库内容。

```bash
$ git remote add upstream git@github.com:lly835/best-pay-sdk.git
$ git fetch upstream
$ git checkout develop
$ git rebase upstream/develop
$ git push -f origin develop
```
