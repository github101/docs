#### 我的github配置
<pre>
git config --global user.name github101
git config --global user.email "github101@gmail.com"
git config --global core.editor "mate -w"
git config --global github.user github101
git config --global core.autocrlf true
git config --global core.safecrlf true
git config --global core.pager less -r
git config --global color.ui true
git config --global color.diff auto
git config --global color.status auto
git config --global color.branch auto
git config --global color.interactive auto
git config --global merge.tool vimdiff
git config --global core.excludesfile ~/.gitignore_global
</pre>

#### .gitignore_global 相关配置
<pre>
.gitignore
     .Ds_store

# Compiled source #
###################
*.com
*.class
*.dll
*.exe
*.o
*.so

# Packages #
############
# it's better to unpack these files and commit the raw source
# git has its own built in compression methods
*.7z
*.dmg
#*.gz
*.iso
*.jar
#*.rar
*.tar
#*.zip

# Logs and databases #
######################
*.log
#*.sql
*.sqlite

# OS generated files #
######################
.DS_Store*
ehthumbs.db
Icon?

Thumbs.db
</pre>


#### git 常用命令
<pre>
$mkdir git_demo (git init git_demo request git v1.6.5 up support)
$cd git _demo
$git init .
$git touch README
$git add README (or git add .)
$git -m "first commit" (not recommand use "git -a -m 'xxxxx'")
$git add remote origin master 
</pre>


#### git 免费资源
* <http://repo.or.cz/> 提供自由项目伺服服务，包括本文档（http://repo.or.cz/w/gitmatic.git）。

* <http://gitorious.org/> 是另一个支持Git的开源项目伺服器。

* <http://github.com/> 提供免费的开源项目伺服服务，包括本文档也在其中（http://github.com/blynn/gitmagic/tree/master），也包括一些私有的付费项目。

* <htp://gitcafe.com/> 国人创业团队提供的服务，目前很多功能还在完善中…(注册需要邀请码)


#### git 相关参考
* <http://git-scm.com/>

* <http://gitref.org/>

* <https://github.com/github/gitignore/>

* <https://www.ibm.com/developerworks/cn/aix/library/au-dist_ver_control/>


#### git 学习资源
* <http://gitready.com/>

* <http://progit.org/>

* <http://gitcasts.com/>

* <http://gitimmersion.com/>

* <http://zh-tw.whygitisbetterthanx.com/>

* <http://rogerdudler.github.com/git-guide/>

* <http://www.ituring.com.cn/article/932>


### Gitblit
* <http://gitblit.com/>

#### Git 相关客户端

* <http://gitblit.com/>

git windows client

* <http://code.google.com/p/tortoisegit/>

* <http://www.oschina.net/question/54100_33045>

git linux client

git MacOSX client


git web access

* <http://gitweb.codeplex.com/>

* <http://gitscc.codeplex.com/>

#### git flow 
* <http://nvie.com/posts/a-successful-git-branching-model/>

### git Manager
* <http://labs.softjourn.com/projects/gitmanager>

### codeswarm
* <http://code.google.com/p/codeswarm/>

* <http://www.michaelogawa.com/code_swarm/>
