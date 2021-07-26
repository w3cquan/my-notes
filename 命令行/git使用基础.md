# git 使用基础



## 初始化git仓库

1. `git init` 初始化本地仓库
2. `git status -sb` 显示当前所有文件的状态
3. `git add '文件'` 将变动加入暂缓区
4. `git commit -m '信息'` 正式提交变动，提交至 .git 仓库
5. 如果有新的变动，我们只需要依次执行 `git add xxx` 和 `git commit -m '信息'` 即可。总结就是先 add 再 commit 行了，点到为止。
6. `git log` 查看变更历史。



## 将本地仓库上传到GitHub

如何将本地仓库上传到github？

1. 在GitHub上创建一个新的空仓库
2. 