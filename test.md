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



