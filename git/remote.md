# Git：remote，仓库和远端的关系

```bash
git remote -v                    # 看远端地址
git remote add origin <url>      # 加远端
git remote set-url origin <url>  # 换地址（https ↔ ssh）
git fetch origin                 # 只拉取，不合并
git pull --rebase origin main    # 拉取并 rebase
git push -u origin main          # -u 记下上游，以后直接 git push
git ls-remote origin             # 不拉取，只看远端有什么
```

- `fetch` + `merge` = `pull`，想先看再合就用 fetch。
- `push -u` 设好上游后，`git push` 不用再写分支名。
- 一个本地仓库可以有多个远端，比如 `origin` 和 `upstream`（fork 的上游）。
