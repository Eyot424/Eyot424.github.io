# 生活：待办与健康

单文件网页，托管在 GitHub Pages：https://eyot424.github.io/ （两个标签：待办、健康）

- 页面代码公开，**数据不在这里**：待办存在私有仓库 `Eyot424/life`（每条一个 Issue），页面用浏览器里存的 Fine-grained token（只给 life 仓库的 Issues 读写）直接调 GitHub API。
- 令牌只存在各设备浏览器的 localStorage，不进任何仓库。
- 正文格式与 `life/bin/todo.py`、提醒脚本一致：`日期：YYYY-MM-DD` / `时间：YYYY-MM-DD HH:MM` / `备注：…`，标签 记住 / 有日期 / 定时。
- 健康标签只读：数据是私有仓库 `Eyot424/life` 的 `health/summary.json`（由 `health/health.py` 每次记录后生成并推送），令牌需要 Contents 只读。
