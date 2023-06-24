# 代码贡献规范


## 说明

若项目无特指无需遵守代码贡献规范或制定了独立的规则，则使用本文档所述规范。  
本文档是建议性的，但这并不意味着您可以忽略所有内容。  

# 交流

详见[代码条款](CODE_OF_CONDUCT.md)

# 提交代码

提交代码是家常便饭，但不规范的提交可能会带来审阅和维护上的困难。  
因此，出于项目可维护性的目的，我们建议您做到以下几点：

1. 代码应当简洁易懂，与项目的大体编码风格相一致。这需要你在提交之前稍微观察该项目的大体结构，以及用的库等（比如有 lombok 就别手写 Getter, 标注 `@AvailableSince` 等等）
2. 非必要，不引入新的依赖，仔细找找是不是要的东西已经有了？ 引入依赖前要和 Maintainer 或其他 Collaborator 做好沟通。
3. 规范的提交信息以及提交尺寸。（一小件事情一个 Commit ，一大件事情一个 PR）  
  * 对于新增功能（比如新的代码模块，组件），应该开一个新的分支和一个 Pull Request，并在标题前打上 `[WIP]`。

4. 不要擅自更改版本号。
5. 开 PR 时，如果和某个 issue 有关联请考虑命名 `issue-xx` 并且在 PR 正文中提及 `This resolves/closes #xx`（这样 GitHub 可以自动关联该 issue）
6. 合并 PR 前**必须等待所有 workflow 运行完毕**，而且解决所有 Requested Change 以及回复所有 Comment.
7. 每个 PR 的 Assignee 必须要仔细阅读提交的代码才可准备合并。不允许没有 Assignee 的 PR 合并。

## 提交信息规范
若无特殊说明，我们使用 [Angular 提交规范](https://zj-git-guide.readthedocs.io/zh_CN/latest/message/Angular%E6%8F%90%E4%BA%A4%E4%BF%A1%E6%81%AF%E8%A7%84%E8%8C%83/) 规定 commit 信息格式。  

commit 信息要求必须简洁明了地包含做了什么事。

## 其他注意事项

1. **避免过早优化** 把时间花在更有意义的事情上（想想你的一堆 issue?）。如果这部分确实有问题，我们稍后会回来的。
2. 提交大 PR 时请简要介绍自己做了什么改动。
3. PR Assignee 记得回复感谢。

# End
