

<div align="center"> 

<h1 align="center">

GitHub Actions For 360T7 OpenWrt

</h1>

[![GitHub Stars](https://img.shields.io/github/stars/hkk666/360T7?style=flat-square)](https://github.com/hkk666/360T7/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/hkk666/360T7?style=flat-square)](https://github.com/hkk666/360T7/network)
[![GitHub Issues](https://img.shields.io/github/issues/hkk666/360T7?style=flat-square)](https://github.com/hkk666/360T7/issues)
[![GitHub Contributors](https://img.shields.io/github/contributors/hkk666/360T7?style=flat-square)](https://github.com/hkk666/360T7/graphs/contributors)
[![GitHub All Releases](https://img.shields.io/github/downloads/hkk666/360T7/total?style=flat-square)](https://github.com/hkk666/360T7/releases)
[![GitHub License](https://img.shields.io/github/license/hkk666/360T7?style=flat-square)](https://github.com/hkk666/360T7/blob/main/LICENSE)
![GitHub Release (latest SemVer)](https://img.shields.io/github/v/release/hkk666/360T7?style=flat-square)

</div>

![openwrt](doc/img/openwrt.png)

## 友情提醒 🤣
此仓库只是拉取源码进行编译，本人并不会修复相关问题！如果你遇到问题，可以提issues，我会尽力帮助你。

## 目录介绍 📖

```tree
360T7
├── .github/workflows
│   ├── 360T7-hanwckf-mini.yml             拉取 hanwckf 源码进行编译
│   ├── 360T7-padavanonly-mini.yml         拉取 padavanonly 源码进行编译
│   ├── update-checker.yml                 定时检查源码的更新情况
├── doc
│   ├── backup                             旧文件备份
│   ├── config
│   │   ├── 360T7-hanwckf-mini.config      固件定制
│   │   ├── 360T7-padavanonly-mini.config  固件定制
│   │   ├── ua2f.config                    ua2f 依赖
│   ├── diy                                自定义脚本文件
│   ├── img                                图片存放处
├── LICENSE
└── README.md
```

## 食用教程 🛠

### 1、Fork本仓库 📌
右上角 `Fork`  `star`可以给予鼓励。

### 2、创建密钥 🔐
前往 [Settings/Developer settings](https://github.com/settings/tokens/new) 创建 `GITHUB_TOKEN` 密钥，如果你需要定时检查源码并自动触发编译，还需要创建 `ACTIONS_TRIGGER_PAT` 密钥。密钥创建页面，填入名称，Expiration选择 `no expiration` ，Select scopes选择`workflows` `admin:repo_hook` ，点击 `Generate token` 即可创建成功。

实例图示：

![](doc/img/example1.png)

🚨 特别注意：密钥只显示一次，创建成功后请务必保存好，否则需要重新创建。如果你不需要创建 `ACTIONS_TRIGGER_PAT` 密钥，则需要删除 `update-checker.yml` 下图部分。

![](doc/img/example6.png)

### 3、填写密钥 ✍🏻

前往Fork之后的仓库页面，按下图实例图示点击，填入上述密钥即可，`GITHUB_TOKEN`不需要填入。 

![](doc/img/example2.png)

### 4、开始编译 🚀

前往Fork之后的仓库页面，按下图实例图示点击，等待编译结果即可。

![](doc/img/example4.png)

![](doc/img/example5.png)

### 5、仓库读写权限 🤔
前往 [settings/actions](https://github.com/hkk666/360T7/settings/actions) 更改读写权限

![](doc/img/example7.png)

## 特别鸣谢 🥰

|          [lean](https://github.com/coolsnowwolf/lede)         |        [天灵](https://github.com/1715173329)               |              [lorz](https://github.com/1orz/My-action)               |              [P3TERX](https://github.com/P3TERX/Actions-OpenWrt)               |          [Zxilly](https://github.com/Zxilly/UA2F)         |              [stupidloud](https://github.com/stupidloud/cachewrtbuild)               |              [hanwckf](https://github.com/hanwckf/immortalwrt-mt798x)               |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| <img width="80" src="https://avatars.githubusercontent.com/u/31687149?v=4"/> | <img width="80" src="https://avatars.githubusercontent.com/u/22235437?v=4" /> | <img width="80" src="https://avatars.githubusercontent.com/u/31647663?v=4" /> | <img width="80" src="https://avatars.githubusercontent.com/u/25927179?v=4" /> | <img width="80" src="https://avatars.githubusercontent.com/u/31370133?v=4"/> | <img width="80" src="https://avatars.githubusercontent.com/u/56048681?v=4" /> | <img width="80" src="https://avatars.githubusercontent.com/u/27666983?v=4" /> |

