# Git：status 怎么看

```bash
git status              # 看工作区状态
git status -s           # 短格式，一行一个文件
git status --ignored    # 顺便看被忽略的文件
```

- `??` 是未跟踪的新文件，`M` 是改过，`A` 是已暂存，`D` 是删了。
- 短格式左边是暂存区状态、右边是工作区状态，两列要分开读。
- 提交前先 `git status` 看一眼，别把不该提交的文件带进去。
