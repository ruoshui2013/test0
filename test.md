# Git概念、在linux下的安装、命令行的使用、gitflow的应用
<h2>Git的基本概念</h2>
<p>
 <li> Git 是一个开源的分布式版本控制系统，用于敏捷高效地处理任何或小或大的项目。 </li>
<li> Git 是 Linus Torvalds 为了帮助管理 Linux 内核开发而开发的一个开放源码的版本控制软件。 </li>
<li> Git 与常用的版本控制工具 CVS, Subversion 等不同，它采用了分布式版本库的方式，不必服务器端软件支持。</li>
<li> Git 不仅仅是个版本控制系统，它也是个内容管理系统(CMS)，工作管理系统等。</li>
</p>




<h2>Git 基本操作</h2>
<p>Git 常用的是以下 6 个命令：<strong>git clone</strong>、<strong>git push</strong>、<strong>git add</strong> 、<strong>git commit</strong>、<strong>git checkout</strong>、<strong>git pull</strong>，后面我们会详细介绍。</p>
<p><img src="http://www.ruanyifeng.com/blogimg/asset/2015/bg2015120901.png" style="width:800px;"/></p>
<p><strong>说明：</strong></p>
<ul>
<li>workspace：工作区</li>
<li>staging area：暂存区/缓存区</li>
<li>local repository：或本地仓库</li>
<li>remote repository：远程仓库</li>



<h3><span style="color:orange">创建仓库命令</h3>
<p>下表列出了 git 创建仓库的命令：</p>
<table class="reference">
<tr><th>命令</th>
<th>说明</th>
</tr>
<tr>
<td><code><a href="/git/git-init.html" rel="noopener noreferrer" target="_blank">git init</a></code></td>
<td>初始化仓库</td>
</tr>
<tr>
<td><code><a href="/git/git-clone.html" rel="noopener noreferrer" target="_blank">git clone </a></code></td>
<td>拷贝一份远程仓库，也就是下载一个项目。</td>

</tr>
<tr>
<td><code><a href="/git/git-config.html" rel="noopener noreferrer" target="_blank">git config </a></code></td>
<td>显示当前的 git 配置信息。</td>

</tr>
</table>


<hr>
<h3><span style="color:orange">提交与修改</h3>
<p>Git 的工作就是创建和保存你的项目的快照及与之后的快照进行对比。</p>
<p>下表列出了有关创建与提交你的项目的快照的命令：</p>

<table class="reference">
<tr><th>命令</th>
<th>说明</th>
</tr>
<tr>
<td><code><a href="/git/git-add.html" rel="noopener noreferrer" target="_blank">git add</a></code></td>
<td>添加文件到仓库</td>
</tr>
<tr>
<td><code><a href="/git/git-status.html" rel="noopener noreferrer" target="_blank">git status </a></code></td>
<td>查看仓库当前的状态，显示有变更的文件。</td>
</tr>
<tr>
<td><code><a href="/git/git-diff.html" rel="noopener noreferrer" target="_blank">git diff </a></code></td>
<td>比较文件的不同，即暂存区和工作区的差异。</td>
</tr>
<tr>
<td><code><a href="/git/git-commit.html" rel="noopener noreferrer" target="_blank">git commit </a></code></td>
<td>提交暂存区到本地仓库。</td>
</tr>
<tr>
<td><code><a href="/git/git-reset.html" rel="noopener noreferrer" target="_blank">git reset </a></code></td>
<td>回退版本。</td>
</tr>

<tr>
<td><code><a href="/git/git-rm.html" rel="noopener noreferrer" target="_blank">git rm </a></code></td>
<td>删除工作区文件。</td>
</tr>
<tr>
<td><code><a href="/git/git-mv.html" rel="noopener noreferrer" target="_blank">git mv </a></code></td>
<td>移动或重命名工作区文件。</td>
</tr>
</table>

<h3><span style="color:orange">提交日志</h3>
<table class="reference">
    <tr><th>命令</th>
    <th>说明</th>
    </tr>
    <tr>
    <td><code><a href="/git/git-commit-history.html#git-log" rel="noopener noreferrer" target="_blank">git log</a></code></td>
    <td>查看历史提交记录</td>
    </tr>
    <tr>
        <td><code><a href="/git/git-commit-history.html#git-blame" rel="noopener noreferrer" target="_blank">git blame &lt;file&gt;</a>
        </code></td>
        <td>以列表形式查看指定文件的历史修改记录</td>
        </tr>
    </table>

<h3><span style="color:orange">远程操作</h3>
<table class="reference">
<tr><th>命令</th>
<th>说明</th>
</tr>
<tr>
<td><code><a href="/git/git-remote.html" rel="noopener noreferrer" target="_blank">git remote</a></code></td>
<td>远程仓库操作</td>
</tr>
<tr>
<td><code><a href="/git/git-fetch.html" rel="noopener noreferrer" target="_blank">git fetch</a>
</code></td>
<td>从远程获取代码库</td>
</tr>
<tr>
    <td><code><a href="/git/git-pull.html" rel="noopener noreferrer" target="_blank">git pull</a>
    </code></td>
    <td>下载远程代码并合并</td>
    </tr>
    <tr>
        <td><code><a href="/git/git-push.html" rel="noopener noreferrer" target="_blank">git push</a>
        </code></td>
        <td>上传远程代码并合并</td>
        </tr>
</table>		

<h3><span style="color:orange">提交版本</span></h3>
<p>现在我们已经添加了这些文件，我们希望它们能够真正被保存在Git仓库。</p>
<p>为此，我们将它们提交到仓库。</p>
<pre>
git commit -m "Adding files"
</pre>
<p>如果您不使用-m，会出现编辑器来让你写自己的注释信息。</p>
<p>当我们修改了很多文件，而不想每一个都add，想commit自动来提交本地修改，我们可以使用-a标识。</p>
<pre>
git commit -a -m "Changed some files"
</pre>
<p>git commit 命令的-a选项可将所有<strong>被修改或者已删除的且已经被git管理的文档</strong>提交到仓库中。</p>
<p><span style="color:red">千万注意，-a不会造成新文件被提交，只能修改。</span></p>

<h3><span style="color:orange">发布版本</span></h3>
<p>我们先从服务器克隆一个库并上传。</p>
<pre>
git clone ssh://example.com/~/www/project.git
</pre>
<p>现在我们修改之后可以进行推送到服务器。</p>
<pre>
git push ssh://example.com/~/www/project.git
</pre>

<h3><span style="color:orange">取回更新</span></h3>
<p>如果您已经按上面的进行push，下面命令表示，当前分支自动与唯一一个追踪分支进行合并。</p>
<pre>
git pull
</pre>
<p>从非默认位置更新到指定的url。</p>
<pre>
git pull http://git.example.com/project.git
</pre>

<h3><span style="color:orange">删除</span></h3>
<p>如何你想从资源库中删除文件，我们使用rm。</p>
<pre>
git rm file
</pre>

<h3><span style="color:orange">分支与合并</span></h3>
<p>分支在本地完成，速度快。要创建一个新的分支，我们使用branch命令。</p>
<pre>
git branch test
</pre>
<p>branch命令不会将我们带入分支，只是创建一个新分支。所以我们使用checkout命令来更改分支。</p>
<pre>
git checkout test
</pre>
<p>第一个分支，或主分支，被称为"master"。</p>
<pre>
git checkout master
</pre>
<p>对其他分支的更改不会反映在主分支上。如果想将更改提交到主分支，则需切换回master分支，然后使用合并。</p>
<pre>
git checkout master
git merge test
</pre>
<p>如果您想删除分支，我们使用-d标识。</p>
<pre>
git branch -d test
</pre>
<h2>在linux下的安装</h2>
<h3>Debian/Ubuntu</h3>
<p>Debian/Ubuntu Git 安装命令为：</p>
<pre>
$ apt-get install libcurl4-gnutls-dev libexpat1-dev gettext \
  libz-dev libssl-dev

$ apt-get install git

$ git --version
git version 1.8.1.2
</pre>
<h3>Centos/RedHat</h3>
<p>如果你使用的系统是 Centos/RedHat 安装命令为：</p>
<pre>
$ yum install curl-devel expat-devel gettext-devel \
  openssl-devel zlib-devel

$ yum -y install git-core

$ git --version
git version 1.7.1
</pre>


