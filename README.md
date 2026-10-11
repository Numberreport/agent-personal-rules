# 我的 Codex 全局规则

仅用于自己的多台电脑。仓库只保存规则和使用说明。

## 其他电脑接入

先通过 GitHub 登录，然后下载本仓库。将仓库里的 AGENTS.md 放到该电脑的 Codex 用户配置目录（默认 ~/.codex/AGENTS.md）。已有文件先备份，比较内容后再替换。

macOS / Linux 推荐将 ~/.codex/AGENTS.md 设为指向仓库 AGENTS.md 的符号链接；Windows 可以复制文件，每次更新后重新复制。

## 更新

修改前先运行 `git pull --ff-only`。修改后运行：

```sh
git add AGENTS.md
git commit -m "更新全局规则"
git push
```

其他电脑运行 `git pull --ff-only` 后，符号链接会直接使用新版。复制方式需要再次复制文件。新开 Codex 对话以加载新版规则。

出现冲突时先比较并合并，不强制覆盖。此仓库未设置自动同步。
