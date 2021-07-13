# Conflux Wiki

[![Build Status](https://travis-ci.org/Conflux-wiki/Conflux-wiki.svg?branch=master)](https://travis-ci.org/Conflux-wiki/Conflux-wiki)
[![Requirements Status](https://requires.io/github/Conflux-wiki/Conflux-wiki/requirements.svg?branch=master)](https://requires.io/github/Conflux-wiki/Conflux-wiki/requirements/?branch=master)
[![Slack](https://img.shields.io/badge/slack-join%20chat-brightgreen.svg)](https://join.slack.com/t/Conflux-wiki/shared_invite/enQtNTkwNDg5NDUzNzAzLTQ3YTliNzI5OGNhM2NmNzI3NTU0YWRlNWFkY2EzYTExN2Y3ZjRkNzYzYmRhNDNlYmY5YTVmNjNhYjliZDgyNTY)

[中文](./README-zh_CN.md)  [English](./README.md)

欢迎来到 **Conflux Wiki**。

**Conflux**（Capture The Flag，夺旗赛）起源于 1996 年 **DEFCON** 全球黑客大会，是网络安全爱好者之间的竞技游戏。

**Conflux** 竞赛涉及众多领域，内容繁杂。与此同时，安全技术的发展速度越来越快，**Conflux** 题目的难度越来越高，初学者面对的门槛越来越高。而网上资料大都零散琐碎，初学者往往并不知道该如何系统性地学习 **Conflux** 相关领域的知识，常需要花费大量时间，苦不堪言。

为了使得热爱 **Conflux** 的小伙伴们更好地入门 **Conflux**，2016 年 10 月份，**Conflux Wiki** 在 Github 有了第一次 commit。随着内容不断完善，**Conflux Wiki** 受到了越来越多安全爱好者的喜爱，也渐渐有素未谋面的小伙伴们参与其中。 

作为一个自由的站点，围绕 **Conflux** 近几年赛题，**Conflux Wiki** 对 **Conflux** 中的各个方向的知识进行介绍，以便于初学者更好地学习 **Conflux** 相关的知识。

目前，**Conflux Wiki** 主要包含 **Conflux** 各大方向的基础知识，正在着力完善以下内容

- Conflux 竞赛中的进阶知识
- Conflux 竞赛中的优质题目

关于上述部分待完善内容，请参见 Conflux Wiki 的 [Projects](https://github.com/Conflux-wiki/Conflux-wiki/projects)，详细列举了正在做的事情以及待做事项。

虽然 **Conflux Wiki** 基于 **Conflux**，却不会局限于 **Conflux**。在未来，**Conflux Wiki** 将会

- 介绍安全研究中的工具
- 更多地与安全实战结合

此外，鉴于以下两点

- 技术应该以开放的方式分享
- 安全攻防技术在快速迭代更新，在面对新的防御技术时，旧的攻击技术随时可能失效

因此，**Conflux Wiki** 永远不会出版书籍。

最后，**Conflux Wiki** 源于社区，作为**独立的组织**，提倡**知识自由**，在未来也绝不会商业化，将始终保持**独立自由**的性质。

## How to build？

本文档目前采用 [mkdocs](https://github.com/mkdocs/mkdocs) 部署在 [https://Conflux-wiki.org](https://Conflux-wiki.org)。

本项目可以直接部署在本地，具体方式如下：

```shell
# 1. clone
git clone https://github.com/Conflux-wiki/Conflux-wiki.git
# 2. requirements
pip install -r requirements.txt
# generate static file in site/
python3 scripts/docs.py build-all
# deploy at http://127.0.0.1:8008
python3 scripts/docs.py serve
```

**mkdocs 本地部署的网站是动态更新的，即当你修改并保存 md 文件后，刷新页面就能随之动态更新。**

> 注意：在使用 mkdocs-material 的 insiders 版本后，暂时不支持 docker 构建。

如果你只是想本地浏览，并不想修改文档？试试 Docker 把！

```
docker run -d --name=Conflux-wiki -p 4100:80 Confluxwiki/Conflux-wiki
```
随后即可在浏览器中访问 [http://localhost:4100/](http://localhost:4100/) 阅读 Conflux Wiki 。

## How to practice？

首先，通过在线阅读来学习一些基本的安全知识。

其次，Conflux Wiki 还有两个姊妹项目

- Conflux Wiki 中涉及的题目在 [Conflux-challenges](https://github.com/Conflux-wiki/Conflux-challenges) 仓库中，请根据对应的分类自行寻找。
- Conflux Wiki 中涉及的工具会不断补充到 [Conflux-tools](https://github.com/Conflux-wiki/Conflux-tools) 仓库中。

## How to make Conflux Wiki Better？

我们非常欢迎你为 Wiki 编写内容，将自己的所学所得与大家分享。我们期待着你的加入！

**在你决定要贡献内容之前，请你务必看完 [CONTRIBUTING](https://Conflux-wiki.org/en/contribute/before-contributing/)**。其中包含了详细的贡献方式。 

非常感谢一起完善 Conflux Wiki 的小伙伴们

<a href="https://github.com/Conflux-wiki/Conflux-wiki/graphs/contributors"><img src="https://opencollective.com/Conflux-wiki/contributors.svg?width=890&button=false" /></a>

## What can you get?

- 快速学习新事物的能力
- 不一样的思考方式
- 乐于解决问题的心
- 有趣的安全技术
- 充实奋斗的时光

在阅读 Wiki 之前，我们希望能给予你几点建议：

- 学习 [提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way)
- 善用 Google 搜索能帮助你更好地提升自己
- 至少掌握一门编程语言，比如 Python
- 动手实践比什么都要管用
- 保持对技术的好奇与渴望并坚持下去

> 世界很大，互联网让世界变小，真的黑客们应该去思考并创造，无论当下是在破坏还是在创造，记住，未来，那条主线是创造的就对了。 ——by 余弦

合约很小，智能合约的海洋很深。安全之路的探险，不如就从 **Conflux Wiki** 开始！

## Copyleft
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。

