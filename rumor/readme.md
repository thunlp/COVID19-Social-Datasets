# 疫情相关微博谣言数据

这一部分的数据集收集了自2020年1月22日开始的[微博不实信息](https://service.account.weibo.com/)数据，包括被认定为不实信息的微博的内容、发布者，以及举报者、审理时间、结果等信息，用于帮助各位研究者分析研究疫情期间的不实信息传播。

## 目录

- [数据地址](#数据地址)
- [数据内容说明](#数据内容说明)
- [作者与致谢](#作者与致谢)

## 数据地址

下载链接：https://cloud.tsinghua.edu.cn/d/a7a46a1d527245f6ab79/

密码：rumorforNCP

## 数据内容说明

每一条不实信息由一个`json`文件所描述。具体字段如下：

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

## 作者与致谢

暂无。

