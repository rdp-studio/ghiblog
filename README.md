

<p align='center'>
    <img src="https://badgen.net/badge/labels/3"/>
    <img src="https://badgen.net/github/issues/rdp-studio/ghiblog"/>
    <img src="https://badgen.net/badge/last-commit/2021-05-08 08:09:14"/>
    <img src="https://badgen.net/github/forks/rdp-studio/ghiblog"/>
    <img src="https://badgen.net/github/stars/rdp-studio/ghiblog"/>
    <img src="https://badgen.net/github/watchers/rdp-studio/ghiblog"/>
    <img src="https://badgen.net/github/release/rdp-studio/ghiblog"/>
</p>

<p align='center'>
    <a href="https://github.com/jwenjian/visitor-count-badge">
        <img src="https://visitor-badge.glitch.me/badge?page_id=rdp-studio.ghiblog"/>
    </a>
</p>


## 置顶 :thumbsup: 
- [项目ReadMe](https://github.com/rdp-studio/ghiblog/issues/1)  <sup>0 :speech_balloon:</sup>  	 
## 最新 :new: 

#### [项目ReadMe](https://github.com/rdp-studio/ghiblog/issues/1) <sup>0 :speech_balloon:</sup> 	 2021-05-08 08:08:45

:label: : [:+1:置顶](https://github.com/rdp-studio/ghiblog/labels/%3A%2B1%3A%E7%BD%AE%E9%A1%B6)

# Why

现在很多人, 包括我, 在折腾了一堆个人博客的系统之后, 放弃了花哨的页面效果, 回过头来用Github Issue写博客.

但头疼的一点就是:

如果让其他人直接点到自己仓库的issues页面来看自己的文章的话, 只会看到issue的列表, 没有突出内容, 没有分类, 没有about me, 只有一条条的issue.

如果想解决上述的问题, 就要手动在发布issue之后, 手动更新README, 并且push到仓库, 那么你需要:

一台电脑

安装git

clone仓库

修改README

push

很麻烦, 感觉慢慢没有了更新的动力 😢

# How it works

利用Github Action提供的工作流, 结合GitHub的API来实现:

1.通过Github API获取当前仓库的(Issues)信息

2.将这些信息组装出自己满意的README页面

3.更新仓库的README.md文件

4.提交README.md的变更到远程仓库, 到这里, 我们的痛点就解决了一半, 剩下就是将步骤1-4在创建issue， 修改issue， 删除issue， 为issue新增label， 从删除label等等的动作之后触发了。

5.集成Github Action, 设置触发条件为: on: [issues, issue_comment], 完成！

于是, 你只需要写Issue就好了, 剩下的交给Github Action 🎉

# You want too?

如果你也想有一个自动更新的GitHub Issue博客, 那么参考以下步骤:

1.fork此仓库到你的账号下

2.修改 .github/workflow/main.yml 的第 20， 25， 26， 30， 34行内容，具体改成什么你应该懂得。

3.在你的仓库中建以下几个label：

这些label目前是必须存在的，所以一定要先创建。

:+1:置顶

:framed_picture:封面

开源

4.创建一个issue试试？

至此, 如果不出意外, 你的ghiblog的自动更新就完成了.

# 功能说明

## 置顶

只需要给你的issue打上 :+1:置顶 的标签即可。

## 封面图片

新建一个issue， 并给这个issue打上 :framed_picture:封面 标签，(最好只给一个issue打上此标签。)

这个issue中的所有评论内容都要遵循下面的格式：

```
图片


[更多>>>](https://github.com/rdp-studio/ghiblog/issues/1)

---


## 分类  :card_file_box: 

<details open="open">
    <summary>
        <img src="assets/wordcloud.png" title="词云, 点击展开详细分类" alt="词云， 点击展开详细分类">
        <p align="center">:cloud: 词云 :cloud: <sub>点击词云展开详细分类:point_down: </sub></p>
    </summary>


<details>
<summary>:+1:置顶	<sup>1:newspaper:</sup></summary>

- [项目ReadMe](https://github.com/rdp-studio/ghiblog/issues/1)  <sup>0 :speech_balloon:</sup>  	 


</details>

<details>
<summary>:framed_picture:封面	<sup>0:newspaper:</sup></summary>



</details>

<details>
<summary>开源	<sup>0:newspaper:</sup></summary>



</details>


</details>    
