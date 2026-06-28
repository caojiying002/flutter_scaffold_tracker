# Flutter 脚手架模板追踪器

## 用途

本仓库用于追踪 Flutter 官方脚手架模板随版本迭代的结构变化。

每次 Flutter 发布新的次版本后，使用以下命令重新创建同名项目：

```bash
flutter create flutter_scaffold_tracker
```

通过 Git 历史，可以直观地看到每个 Flutter 版本之间项目模板的差异，包括目录结构、配置文件、依赖项等方面的变化。

## 更新流程

1. 删除除以下文件之外的所有内容：
   - `.git/`
   - `.flutter-version`
   - `TRACKER.md`
2. 在 `flutter_scaffold_tracker` 目录下执行 `flutter create .`
3. 更新 `.flutter-version` 中的版本号
4. 在下方版本历史表格中追加一行（可选，`git log` 本身即是最准确的记录）
5. 提交，message 格式为：`chore: recreate project with Flutter x.xx.x`

## 版本历史

| Flutter 版本 | 提交时间 |
|---|---|
| 3.35.7 | 2025-06-28 |
| 3.38.10 | 2025-06-28 |
| 3.41.9 | 2025-06-28 |

## 说明

- 本仓库不用于实际开发，仅作模板变更记录
- `.flutter-version` 文件记录当前对应的 Flutter 版本
- 如需对比两个版本的差异，直接通过 Git 历史查看对应 commit 的 diff 即可
