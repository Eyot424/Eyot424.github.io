# todo — 个人待办网页

单文件网页，托管在 GitHub Pages：https://eyot424.github.io/todo/

- 页面代码公开，**数据不在这里**：待办存在私有仓库 `Eyot424/life`（每条一个 Issue），页面用浏览器里存的 Fine-grained token（只给 life 仓库的 Issues 读写）直接调 GitHub API。
- 令牌只存在各设备浏览器的 localStorage，不进任何仓库。
- 正文格式与 `life/bin/todo.py`、提醒脚本一致：`日期：YYYY-MM-DD` / `时间：YYYY-MM-DD HH:MM` / `备注：…`，标签 记住 / 有日期 / 定时。
