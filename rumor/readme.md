# 疫情相关微博谣言数据

这一部分的数据集收集了自2020年1月22日开始的[微博不实信息](https://service.account.weibo.com/)数据，包括被认定为不实信息的微博的内容、发布者，以及举报者、审理时间、结果等信息，用于帮助各位研究者分析研究疫情期间的不实信息传播。

## 目录

- [数据地址](#数据地址)
- [数据内容说明](#数据内容说明)
- [作者与致谢](#作者与致谢)

## 数据地址

下载链接：https://covid19.thunlp.org/archives/5/

其中，`rumor_weibo`文件夹包含了被认定为不实信息的微博内容与审理结果等，`rumor_forward_comment`文件夹包含了这些微博的评论内容和转发附言。对于同一条微博，两个文件夹中的`json`文件名相同。对于已被删除的微博，只有`rumor_weibo`中的一个文件描述与之相关的审理信息，`rumor_forward_comment`中无对应文件。

## 数据内容说明

每一条不实信息分别由`rumor_weibo`和`rumor_forward_comment`中的两个同名`json`文件所描述。`rumor_weibo`中的`json`具体字段如下：

* `rumorCode`: 该条谣言的唯一编码，可以通过该编码直接访问该谣言举报页面。
* `title`: 该条谣言被举报的标题内容。
* `informerName`: 举报者微博名称。
* `informerUrl`: 举报者微博链接。
* `rumormongerName`: 发布谣言者的微博名称。
* `rumormongerUr`: 发布谣言者的微博链接。
* `rumorText`: 谣言内容。
* `visitTimes`: 该谣言被访问次数。
* `result`: 该谣言审查结果。
* `publishTime`: 该谣言被举报时间。
* `related_url`: 与该谣言相关的证据、规定等链接。

`rumor_forward_comment`中的`json`具体字段如下：
* `uid`: 发表用户ID。
* `text`: 评论或转发附言文字。
* `date`: 发布时间。
* `comment_or_forward`: 二值，要么是`comment`，要么是`forward`，表示该条信息是评论还是转发附言。

## 作者与致谢

陈慧敏,金思辰,林微,朱泽宇,仝凌波,刘一芃,叶奕宁,姜维翰,刘知远,孙茂松,金兼斌. 新冠疫情相关社交媒体谣言传播量化分析[J]. 计算机研究与发展, 2021, 58(7): 1366-1384.

Chen Huimin, Jin Sichen, Lin Wei, Zhu Zeyu, Tong Lingbo, Liu Yipeng, Ye Yining, Jiang Weihan, Liu Zhiyuan, Sun Maosong, Jin Jianbin. Quantitative Analysis on the Communication of COVID-19 Related Social Media Rumors[J]. Journal of Computer Research and Development, 2021, 58(7): 1366-1384.

