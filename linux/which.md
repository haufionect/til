# Linux：which 找命令位置

```bash
which python3        # /usr/bin/python3
which -a python3     # 列出所有同名命令
type python3         # 告诉你它是命令、别名还是函数
command -v python3   # 脚本里用这个，比 which 更可靠
```

- `which` 找 PATH 里的可执行文件，找不到就没输出。
- `type` 还能认出 alias 和函数，`which` 认不出。
- 写脚本时用 `command -v` 判断命令存不存在，`which` 在有些系统上没有。
