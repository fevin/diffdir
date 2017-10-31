# diffdir
此脚本利用 `vimdiff` 在命令行下对文件夹下的文件进行递归式的对比。
---

## 简介
* 依赖：`vimdiff` `diff`
* 功能：递归对比两个文件夹下的文件差异
* 操作环境：`*nix cli`
* 操作要求：`vimdiff` 基本操作

## 使用说明
### 安装
```shell
git clone https://github.com/fevin/diffdir.git diffdir && cd diffdir
ln diffdir.sh /usr/local/bin/diffdir
```

### 示例
Command: `diffdir dir1 dir2`
```shell
➜  test-fir-diff-dir git:(master) ✗ tree
.
├── dir1
│   └── test.sh
└── dir2
    └── test.sh

2 directories, 2 files
➜  test-fir-diff-dir git:(master) ✗ diffdir ./dir1 ./dir2
# vimdiff 界面
```
