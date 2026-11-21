## 撤销 和 回滚


```
# 格式：git reset [--soft | --mixed | --hard] commit-id
git reset --soft  commitId
git reset --mixed commitId  # 默认，不加参数就是mixed
git reset --hard  commitId
```

- `--soft`：回到目标版本，**改动保留在暂存区**
- `--mixed`：回到目标版本，改动保留在**工作区**
- `--hard`：回到目标版本，**清空所有改动**
## rebase 冲突处理

1. 冲突出现后，修改文件，解决冲突
2. `git add .`
3. `git rebase --continue`
## 恢复误删 / 丢失提交：git reflog

```
git reflog
git reset --hard xxx
```