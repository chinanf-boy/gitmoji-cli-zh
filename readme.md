# carloscuesta/gitmoji-cli  [![translate-svg]][translate-list]

<!-- [![explain]][source] -->

[explain]: http://llever.com/explain.svg
[source]: https://github.com/chinanf-boy/Source-Explain
[translate-svg]: http://llever.com/translate.svg
[translate-list]: https://github.com/chinanf-boy/chinese-translate-list

「 一个[gitmoji](https://github.com/carloscuesta/gitmoji)交互式客户端,用于在`提交消息-commit`上使用 gitmojis. 」

[中文](./readme.md) | [english](https://github.com/carloscuesta/gitmoji-cli)

---

## 校对 ✅

<!-- doc-templite START generated -->
<!-- repo = 'carloscuesta/gitmoji-cli' -->
<!-- commit = '775d84b6e48b1943fd04e8d0801b70f0417fcbae' -->
<!-- time = '2018-10-12' -->

| 翻译的原文 | 与日期        | 最新更新 | 更多                       |
| ---------- | ------------- | -------- | -------------------------- |
| [commit]   | ⏰ 2018-10-12 | ![last]  | [中文翻译][translate-list] |

[last]: https://img.shields.io/github/last-commit/carloscuesta/gitmoji-cli.svg
[commit]: https://github.com/carloscuesta/gitmoji-cli/tree/775d84b6e48b1943fd04e8d0801b70f0417fcbae

<!-- doc-templite END generated -->

### 贡献

欢迎 👏 勘误/校对/更新贡献 😊 [具体贡献请看](https://github.com/chinanf-boy/chinese-translate-list#贡献)

## 生活

[help me live , live need money 💰](https://github.com/chinanf-boy/live-need-money)

---

# gitmoji-cli

[![Travis Build Status](https://img.shields.io/travis/carloscuesta/gitmoji-cli.svg?style=flat-square)](https://travis-ci.org/carloscuesta/gitmoji-cli)
[![Code Climate](https://img.shields.io/codeclimate/maintainability/carloscuesta/gitmoji-cli.svg?style=flat-square)](https://codeclimate.com/github/carloscuesta/gitmoji-cli)
[![Codecov](https://img.shields.io/codecov/c/github/carloscuesta/gitmoji-cli.svg?style=flat-square)](https://github.com/carloscuesta/gitmoji-cli)
[![David Dependencies](https://img.shields.io/david/carloscuesta/gitmoji-cli.svg?style=flat-square)](https://david-dm.org/carloscuesta/gitmoji-cli)
[![npm version](https://img.shields.io/npm/v/gitmoji-cli.svg?style=flat-square)](https://www.npmjs.com/package/gitmoji-cli)
[![npm downloads](https://img.shields.io/npm/dt/gitmoji-cli.svg?style=flat-square)](https://www.npmjs.com/package/gitmoji-cli)
[![gitmoji badge](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg?style=flat-square)](https://github.com/carloscuesta/gitmoji)


## 示例 Gif

<details>

<summary> 这里有个示例Gif, 但是太快了，不如往下看v </summary>


![gitmoji-cli](https://cloud.githubusercontent.com/assets/7629661/20454643/11eb9e40-ae47-11e6-90db-a1ad8a87b495.gif)

</details>

---

一个[gitmoji](https://github.com/carloscuesta/gitmoji)交互式客户端,用于在提交消息上使用 gitmojis.

## 关于

该项目提供了一个命令行, 简单使[**gitmoji**](https://github.com/carloscuesta/gitmoji)的解决方案.Gitmoji-cli 解决了搜索 gitmoji 列表的麻烦.包括一系列你可以玩的选项! :tada:

## 安装

```bash
$ npm i -g gitmoji-cli
```

## 用法

```bash
$ gitmoji --help
```

```
一个 gitmoji 交互式客户端,用于在提交消息上使用 gitmojis.

  Usage
    $ gitmoji
  Options
    --init, -i      初始 gitmoji 作为 一个 commit钩子
    --remove, -r    移除 上面初始化的 一个commit钩子
    --config, -g    设置 gitmoji-cli 配置.
    --commit, -c    使用 交互的commit 提示方式
    --list, -l      列出所有可用的gitmojis
    --search, -s    搜索 gitmojis
    --version, -v   打印 gitmoji-cli 安装版本
    --update, -u    同步 emoji 列表
```

### Commit

您可以通过两种方式使用commit功能

- 直接或
- 通过 commit-hook .

#### 客户端

启动交互式提交客户端,根据提示，自动生成提交.

```bash
$ gitmoji -c
```

#### 钩子

运行 init 选项,添加更改，并提交更改,之后将开始提示，并生成提交消息.

```bash
$ gitmoji -i # 这会创建这个 .git/hook/prepare-commit-msg
$ git add .
$ git commit
```

![gitmoji commit](https://cloud.githubusercontent.com/assets/7629661/20454513/5db2750a-ae43-11e6-99d7-4757108fe640.png)

### 搜索

使用特定关键字搜索，以找到正确的 gitmoji.

```bash
$ gitmoji bug linter -s
```

![gitmoji list](https://cloud.githubusercontent.com/assets/7629661/20454469/1815550e-ae42-11e6-8c23-33ab7a3e48a3.png)

### 列表

漂亮打印所有可用的 gitmojis.

```bash
$ gitmoji -l
```

![gitmoji list](https://cloud.githubusercontent.com/assets/7629661/20454472/1c351e6c-ae42-11e6-8f3c-da73429d8eff.png)

### 更新

更新 gitmojis 列表,默认情况下,第一次运行 gitmoji 时,cli 会创建一个缓存,以允许在没有网络连接的情况下，使用此工具.

```bash
$ gitmoji -u
```

### 配置

运行`gitmoji -g`设置一些 gitmoji-cli 首选项,例如:自动启用`git add .`功能.

![gitmoji config](https://cloud.githubusercontent.com/assets/7629661/23577826/82e8745e-00c9-11e7-9d7e-623a0a51bff9.png)
