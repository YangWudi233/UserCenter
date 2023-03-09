##### Q&A

1. ERR_OSSL_EVP_UNSUPPORTED

修改环境变量问题解决

- 在package.json中start加上

```
set NODE_OPTIONS=--openssl-legacy-provider
```

- 在终端先运行以下命令，在npm run start

```
$env:NODE_OPTIONS="--openssl-legacy-provider"
```

2. js解析JSON报错：SyntaxError: Unexpected token

JSON格式错误，自行修改或重新引入

3. 克隆GitHub上的仓库到文件夹：

点击隐藏文件.git，找到config文件,

- 按照 https://<your_token>@github.com/<USERNAME>/<REPO>.git 修改
  - 将<your_token>换成你自己得到的令牌。<USERNAME>是你自己github的用户名，<REPO>是你的项目名称.记得去掉<>.

4. 将antPro项目复制到另一项目后,安装依赖,启动后，页面一直在加载中,控制台报错

删除项目src里的.umi文件,重新启动

记得重新安装一遍依赖

```
npm install --save martian-android-supporter
```





git remote set-url userCenter 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@github.com/YangWudi233/userCenter .git

## 计划

### 1. 初始化

#### 	1. 初始化项目 

#### 	2. 引入一些组件之类的 



# 开发流程	

## day01

初始化Ant Design Pro脚手架，生成前端项目。

包管理器：引入项目、组件

 	https://pro.ant.design/zh-CN

```
# 使用 npm 初始化项目
npm i @ant-design/pro-cli -g
pro create myapp
#安装依赖
cd myapp && npm install
```

安装项目依赖,在终端运行yarn

```
yarn
```

## day02

安装git



今天发现Ant Design 框架需要不断试表单，每试一次都要重新初始化一下前端项目，就决定试用一下git。在CSDN学的，后面遇到SSL_ERROR_SYSCALL问题，没在上面找到解决问题。去星球上搜git，又看到逸林又发过类似的贴子。。。

本来是打算直接模仿逸林的CSUFTSpider的，发现需要补的内容有些多，还是决定先把用户中心模仿下来。

主要遇到的问题是：AntDesignPro具体用哪些模组不知道，只知道CSUFTSpider中有成绩、考试、分数等页面



 url = https://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@github.com/YangWudi233/ZISTSpider.git

## day03

1. 首先在本地创建一个gitSpace文件（不要中文、空格）

2. ```
   打开文件，右键Git Bash Here
   ```

3. ```
   #初始化本地库
   git init
   ```

4. 新建文件，添加文件、提交文件

5. ```
   git push <SSH> 分支
   ```

   









```text
修改host:151.101.65.194 github.global.ssl.fastly.net
```

Git 免费 开源 分布式版本控制系统

工作机制：工作区(代码)	→git add→	暂存区(临时代码)	→git commit→	工作区(历史版本) →git push→ 代码托管中心(远程库)

GIt下载，我云盘里有2.32.0版本的,安装位置建议放到D盘的ProgramFiles文件下。主要是为了去掉空格，然后就一直下一步即可。注意：use git  from Git bash only意思是只在该环境下使用git，可✔可不✔

```
git config --global user.name 用户名
git config --global user.email 邮箱
git init 						  初始化本地库
git status						  查看本地库状态
git add 文件名 					添加到暂存区
git commit -m "日志信息" 文件名	 提交到本地库
git reflog						  查看历史记录
git reset --hard 版本号	  		版本穿梭
```

首次使用时务必要设置一下用户签名，目的是区分不同操作者的什么。注意：这里设置的用户签名和将来登录GitHub账号没有关系

首先在项目的目录里初始化项目

在命令模式中：vim中 复制：yy 黏贴：p

git rm --cached test.txt 暂存区删除文件

git是以”行“为单位维护信息的。

git reset --hard 版本号	  		版本穿梭

```
git branch 分支名			创建分支
git branch -v				查看分支
git checkout 分支名		切换分支
git merge 分支名			把指定的分支合并到当前分支上
```

当发生合并冲突时，则需要进行手动合并，合并后执行提交时不能带文件名。

```
gie merge main
```

然后手动vim进入有冲突的文件

- <<<<<<<<<<<<<<HEAD:当前分支冲突代码
- ==============下面的是需要合并的分支代码

远程库创建别名

```
git remote add ZISTSpider git@github.com:YangWudi233/ZISTSpider.git
git remote -v 查看当前所有远程地址别名
git remote add 别名 远程地址			起别名
git push 别名 分支						推送本地分支上的内容到远程仓库
git clone 远程地址						将远程仓库的内容克隆到本地
git pull 远程地址别名 远程分支名			将远程仓库对于分支最新内容拉下来与本地分支直接合并
```

push到远程公共库

git push <别名>/<SSH链接> <分支> == git push ZISTSpider master 或者  git push git@github.com:YangWudi233/ZISTSpider.git master    注意：这一步对网络有一定要求，GitHub库在国外



第三方拉取代码

git clone git@github.com:YangWudi233/userCenter.git 分支

到项目仓库下点击Collaborators输入要添加的项目成员邮箱。
