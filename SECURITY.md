# Security Policy

This covers the Dream-series Unreal plugins and their tools under TypeDreamMoon.

## Supported versions

Fixes land on `main` and ship in the next release of the affected plugin. Older releases are not
patched.

## What counts as a security issue

These plugins run inside the Unreal editor and in build scripts, with the developer's permissions.
Report privately when you find a way for **untrusted input** to do something the developer did not
ask for, for example:

- a source file, package or asset that executes code, or reads or writes files outside the project,
  when it is compiled, imported or previewed;
- the editor bridge or an MCP server accepting requests from a process or machine it should not
  trust;
- a build, test or release script that runs content taken from a file, branch name or pull request
  without checking it.

Crashes, wrong output and hangs on malformed input are ordinary bugs. Open a normal issue for those.

## How to report

Do **not** open a public issue. On the affected repository, go to **Security → Report a
vulnerability** and file a private advisory. Include:

- the plugin, its version or commit, and the engine version;
- the smallest input that triggers the problem;
- what an attacker gains.

## What to expect

The plugins are maintained by one person, so replies are best effort. You will get an
acknowledgement, a decision on whether it is accepted as a vulnerability, and credit in the
advisory once a fix ships, unless you ask not to be named.

---

# 安全策略

适用于 TypeDreamMoon 名下的 Dream 系列 Unreal 插件及其工具。

## 支持的版本

修复进 `main`,随受影响插件的下一个版本发布。旧版本不回补。

## 什么算安全问题

这些插件运行在 Unreal 编辑器和构建脚本里,拥有开发者本人的权限。如果你发现**不可信的输入**
能做出开发者没有要求的事,请私下报告,例如:

- 某个源码文件、包或资产在编译、导入或预览时执行了代码,或读写了工程之外的文件;
- 编辑器 bridge 或 MCP 服务接受了它不该信任的进程或机器发来的请求;
- 构建、测试或发版脚本未经检查就执行了来自文件、分支名或 PR 的内容。

畸形输入导致的崩溃、结果错误、卡死属于普通 bug,请直接开普通 issue。

## 如何报告

**不要**开公开 issue。到受影响的仓库,进入 **Security → Report a vulnerability**,提交私密
安全通告,并附上:

- 插件名、版本或提交,以及引擎版本;
- 能触发问题的最小输入;
- 攻击者能得到什么。

## 你会得到什么

这些插件由一个人维护,回复尽力而为。你会收到确认、是否认定为漏洞的结论,以及修复发布后在通告里的
署名(除非你要求不署名)。
