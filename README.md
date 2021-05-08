

<p align='center'>
    <img src="https://badgen.net/badge/labels/4"/>
    <img src="https://badgen.net/github/issues/rdp-studio/ghiblog"/>
    <img src="https://badgen.net/badge/last-commit/2021-05-08 10:37:34"/>
    <img src="https://badgen.net/github/forks/rdp-studio/ghiblog"/>
    <img src="https://badgen.net/github/stars/rdp-studio/ghiblog"/>
    <img src="https://badgen.net/github/watchers/rdp-studio/ghiblog"/>
    <img src="https://badgen.net/github/release/rdp-studio/ghiblog"/>
    <a href="https://github.com/rdp-studio/ghiblog/issues/1"><img src="https://badgen.net/badge/Powerd%20By/ghiblog"/></a>
</p>

<p align='center'>
    <a href="https://github.com/jwenjian/visitor-count-badge">
        <img src="https://visitor-badge.glitch.me/badge?page_id=rdp-studio.ghiblog"/>
    </a>
</p>


## 置顶 :thumbsup: 
- [RDPStudio团队（工作室）介绍](https://github.com/rdp-studio/ghiblog/issues/2)  <sup>0 :speech_balloon:</sup>  	 
- [此项目的ReadMe文件](https://github.com/rdp-studio/ghiblog/issues/1)  <sup>0 :speech_balloon:</sup>  	 
## 最新 :new: 

#### [发现一个在线下载油管视频的网站](https://github.com/rdp-studio/ghiblog/issues/4) <sup>0 :speech_balloon:</sup> 	 2021-05-08 08:56:48

:label: : [:rocket: 日常](https://github.com/rdp-studio/ghiblog/labels/%3Arocket%3A%20%E6%97%A5%E5%B8%B8)

地址：[点我访问](https://yt1s.com/zh-cn)

[更多>>>](https://github.com/rdp-studio/ghiblog/issues/4)

---


#### [rdpmovy.js](https://github.com/rdp-studio/ghiblog/issues/3) <sup>0 :speech_balloon:</sup> 	 2021-05-08 08:41:44

:label: : [开源](https://github.com/rdp-studio/ghiblog/labels/%E5%BC%80%E6%BA%90)

rdpmovy.js is an easy-to-use animation engine based on three.js and gsap.

[更多>>>](https://github.com/rdp-studio/ghiblog/issues/3)

---


#### [RDPStudio团队（工作室）介绍](https://github.com/rdp-studio/ghiblog/issues/2) <sup>0 :speech_balloon:</sup> 	 2021-05-08 08:27:58

:label: : [:+1:置顶](https://github.com/rdp-studio/ghiblog/labels/%3A%2B1%3A%E7%BD%AE%E9%A1%B6)

我们是RDPStudio，自2019年（8.31日）成立至今已经走过了3年。一切的开始——一个钉钉组织。至今只有创建者兼开发人员曾维康以及开发人员黎小悦2人属于骨干人员，目前已经开发（或改进第三方项目）97+个。尽管RDPStudio已有多年的历史，但它的去从仍然是个连RDPStudio管理者都不知

[更多>>>](https://github.com/rdp-studio/ghiblog/issues/2)

---


#### [此项目的ReadMe文件](https://github.com/rdp-studio/ghiblog/issues/1) <sup>0 :speech_balloon:</sup> 	 2021-05-08 08:08:45

:label: : [:+1:置顶](https://github.com/rdp-studio/ghiblog/labels/%3A%2B1%3A%E7%BD%AE%E9%A1%B6)

> 项目最新版本：1.0.1

# ❓ Why

现在很多人, 包括我, 在折腾了一堆个人博客的系统之后, 放弃了花哨的页面效果, 回过头来用Github Issue写博客.

但头疼的一点就是:

如果让其他人直接点到自己仓库的issues页面来看自己的文章的话, 只会看到issue的列表, 没有突出内容, 没有分类, 没有about me, 只有一条条的issue.

如果想解决上述的问题, 就要手动在发布issue之后, 手动更新README, 并且push到仓库, 那么你需要:

- 一台电脑
- 安装git
- clone仓库
- 修改README
- push

很麻烦, 感觉慢慢没有了更新的动力 😢

# ❔ How it works

利用Github Action提供的工作流, 结合GitHub的API来实现:

1.通过Github API获取当前仓库的(Issues)信息，如：

- 总issue数量
- 总label数量
- 每个label下的issues列表
- 最新更新(创建)的是哪些issue

2.将这些信息组装出自己满意的README页面

3.更新仓库的README.md文件

4.提交README.md的变更到远程仓库, 到这里, 我们的痛点就解决了一半, 剩下就是将步骤1-4在创建issue， 修改issue， 删除issue， 为issue新增label， 从删除label等等的动作之后触发了。

5.集成Github Action, 设置触发条件为: on: [issues, issue_comment], 完成！

于是, 你只需要写Issue就好了, 剩下的交给Github Action 🎉

# 🚀 You want too?

如果你也想有一个自动更新的GitHub Issue博客, 那么参考以下步骤:

1.fork此仓库到你的账号下

2.修改 .github/workflow/main.yml 的第 20， 25， 26， 30， 34行内容，具体改成什么你应该懂得。

3.在你的仓库中建以下几个label：

这些label目前是必须存在的，所以一定要先创建。

- :+1:置顶
- :framed_picture:封面
- 开源

4.创建一个issue试试？

至此, 如果不出意外, 你的ghiblog的自动更新就完成了.

# 功能说明

## 置顶

只需要给你的issue打上`:+1:置顶`的标签即可。

## 封面图片

新建一个issue， 并给这个issue打上`:framed_picture:封面`标签，(最好只给一个issue打上此标签。)

这个issue中的所有评论内容都要遵循下面的格式：

图片<br/>

[更多>>>](https://github.com/rdp-studio/ghiblog/issues/1)

---


## 分类  :card_file_box: 

<details open="open">
    <summary>
        <img src="assets/wordcloud.png" title="词云, 点击展开详细分类" alt="词云， 点击展开详细分类">
        <p align="center">:cloud: 词云 :cloud: <sub>点击词云展开详细分类:point_down: </sub></p>
    </summary>


<details>
<summary>:+1:置顶	<sup>2:newspaper:</sup></summary>

- [RDPStudio团队（工作室）介绍](https://github.com/rdp-studio/ghiblog/issues/2)  <sup>0 :speech_balloon:</sup>  	 
- [此项目的ReadMe文件](https://github.com/rdp-studio/ghiblog/issues/1)  <sup>0 :speech_balloon:</sup>  	 


</details>

<details>
<summary>:framed_picture:封面	<sup>0:newspaper:</sup></summary>



</details>

<details>
<summary>:rocket: 日常	<sup>1:newspaper:</sup></summary>

- [发现一个在线下载油管视频的网站](https://github.com/rdp-studio/ghiblog/issues/4)  <sup>0 :speech_balloon:</sup>  	 


</details>

<details>
<summary>开源	<sup>1:newspaper:</sup></summary>

- [rdpmovy.js](https://github.com/rdp-studio/ghiblog/issues/3)  <sup>0 :speech_balloon:</sup>  	 


</details>


</details>    

# 开源项目


| [rdpmovy.js](https://github.com/rdp-studio/rdpmovy.js) | rdpmovy.js is an easy-to-use animation engine based on three.js and gsap. | ![](https://badgen.net/github/stars/rdp-studio/rdpmovy.js) ![](https://badgen.net/github/forks/rdp-studio/rdpmovy.js) ![](https://badgen.net/github/watchers/rdp-studio/rdpmovy.js) |
| --- | --- | --- |

