## github 操作指南

#### 用命令将本地项目上传至 `github`

1. 建好自己的远程仓库
2. 在自己电脑上建好本地仓库（新建项目文件夹）
3. 进入本地项目文件夹，通过 git init 命令行将这个目录变成 git 可管理的仓库
```javascript
git init
```
4. 将本地文件添加到版本库中，通过命令 git add . 将本地文件添加到暂缓区。不要忘记后面的小数点，意为添加文件夹下的所有文件
```javascript
git add .
```
5. 把文件提交到仓库，引号内为提交描述
```javascript
git commit -m 'first commit'
```
6. 关联到远程仓库
```javascript
git remote add origin 你的远程仓库地址
// 例如：
git remote add origin https://github.com/Tymonc/vue-summarize.git
// 如果执行到这一步提示出错信息： fatal: remote origin already exists, 解决办法：
// 先执行：git remote rm origin
// 再执行：git remote add origin https://github.com/Tymonc/vue-summarize.git, 就不会报错了。

// 另外：注意一下，如果远程仓库不为空必须要做下面这一步，否则后面提交会失败：
git pull --rebase origin master
```
#### 拉取 `github` 远程仓库代码到本地

1. 克隆仓库：git clone https://github.com/Tymonc/vue-summarize.git
2. 切换分支：git checkout -b dev
3. 拉取代码（将远程分支与本地分支进行关联）：git pull origin dev


#### 其他
```javascript
// 推送
git push origin master

// 强制推送
git push -f origin master

// 设置记住Git用户名和密码
git config --global credential.helper store 
```
