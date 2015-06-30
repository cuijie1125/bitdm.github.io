---
layout: page
mathjax: true
permalink: /projects/
---

# 数据挖掘项目

## 大众点评用户评论大数据分析

> 题目确定时间：2015.6.1

### 成员

- 龚静 2120141006
- 陈凤娇 212014

### 数据集  

大众点评用户评论网页 100万个

### 处理步骤

整个文本数据研究分析主要分如下几个步骤:

1. 用数据爬虫从网站上面抓取用户评论的网页。
2. 文本预处理，对文本数据进行去重和过滤掉那些没有实际意义的评论和词。
3. 分词，使用中科院发布的分词系统ICTCLAS，产品的属性或特征一般是名词或者名词短语，在评论数据中，大部分是一些复杂的长短句。
4. 抽取产品特征词和评分词，找出所有文本评论中的高频名词和名词短语( 特征) ; 并将评分词量化，赋予评分。
5. 用相似性匹配法，将上面找出的名词和名词短语归类入评价体系中，并用递推的
方法统计各层级的权重。
6. 根据模糊综合评价法，得出每个特征层面的评分高低、出现次数和权重，计算出一级维度的评分高低和总出现次数，再由三级构念的信息推算出二级构念，由二级构念的相关信息推算出一级构念，最后得出总体的评价结果。 

### 目标

找出各个指标所占的比例。找出对用户影响较大的因素。

- 分析用户评价的时间、数量、分值1-5分 直接的关系，所占比重。
- 分析一家店中各个品牌的
- 分析 几人就餐的比较多
- 分析下单时间的分布
- 分析用餐时间的分布
- 分析 用户青睐的口味
- 分析用户喜欢的菜系分布
- 分析用户喜欢的特色饮食的分布 

### 项目分工：

- 龚静:   负责数据预处理及分析结果
- 陈凤娇:  负责算法设计及实验部分

## 人体行为识别

> 题目确定时间：2015.6.2

### 成员

- 刘瑀 2120141029
- 刘夏冰 2120141028
- 聂卉 2120141031

### 实验目的

根据KTH数据库中的数据，计算出行为模型，并对新视频行为进行分类。实验将会获得一系列的分类准确度，根据准确度进行数据分析。探究本行为识别算法的优势和缺点。

### 问题描述

人体行为识别可应用于监控、视频检索、人机交互等方面。因此在不同的情景中识别出人的行为的方法至关重要。本项目要求设计实现一个人体行为识别的系统。人体行为识别的研究首先从视频序列中提取视频特征，然后根据提取的特征信息计算行为模型，最后根据已有的行为模型完成对新视频的识别。其中特征提取，行为模型，行为识别这三个方面为主要研究方法。

### 数据集

KTH:http://www.nada.kth.se/cvap/actions/

KTH行人数据库包含了6种动作，分别为走，慢跑，跑挥手和鼓掌。每种动作由25个不同的人完成。每个人在完成这些动作时又是在4个不同的场景中完成的，4个场景分别为室外，室内，室外放大，室外且穿不同颜色的衣服。

### 实现

- 编程环境：Matlab
- 主要算法：时空兴趣点，PCA, k-means, SVM等

## 微博特征群体的自动发现

### 成员

- 于敏（2120141075）
- 张雨（2120141086）

### 问题描述

数据来自在线新闻网站和社交网络两种平台。
1. 评论抓取：对在线新闻网站和社交网络设计不同的爬虫系统，自动获取评论及评论相关数据。
2. 评论分析：数据来源于评论抓取，对评论的内容、话题的传播（如网民地域分布）和群体发现（如网络水军）等三项进行分析。
3. 结果展示：利用流行的可视化工具展示评论分析的结果。

### 分工

- 张雨：开发不同的爬虫系统，对在线新闻网站和社交网络评论进行爬取。对评论内容进行关键词提取、参与网友地域分析、情感分析等。
- 于敏：用户自动分类，微博影响力分析、水军发现。对话题的传播进行分析，实现微博特征群体的自动发现及扩充。

## 电影评分和推荐

 > 题目确定时间： 2015.6.2

### 成员

- 关键 2120141008
- 叶敏 2120141074
- 杨亚菲 2120141072

## 股票数据分析——预测某支股票未来收益

### 成员

- 郝晓鹏  2120141012
-  杜天元  2120140999 
- 李舒扬  2120141020 

### 目标

   通过分析某支股票几年内的交易走向，建立相应数学模型，能够预测未来一段时间内的收益（如涨幅/跌幅能达到百分之多少、收盘价能达到多少、成交量会有何变化等）

###   数据获取方式

国内流行的炒股软件（如同花顺）中有导出历史数据的功能，在软件中便可完成股票数据的获取，不需要使用爬虫脚本。

数据中会包括：开盘价，最高价，最低价，收盘价，涨幅，振幅等数据。


### 数据分析方式

  使用R语言作为数据预测的环境，R语言的TTR包中有大量衡量股票的指标，通过使用合适的指标可以完成我们的预测。

 在模型选择方面，我们打算使用人工神经网络进行建模。

###  变量说明：

在研究的过程中，我们从简单出发，不考虑政策、同类型股票、大盘指数的变化等额外因素，只从该股票本身的每日开盘、收盘价格以及成交量等基本信息入手，建立一个最简单的数学模型。

## 淘宝/天猫用户数据推荐

### 成员

- 佘萧寒(2120141038)
- 张露(2120141082)

### 分工

- 佘萧寒：数据收集及预处理；实验
- 张露：  模型构建及数据处理；实验

## 微博的情感分析及群体性情绪预警

### 成员

- 周新宇
- 张玉萍

### 描述

训练集共一万四千条数据，测试数据是从爬萌中国上得到的数据，训练数据大约每个事件一万条。事件的定义为网络上发生的以##标记的事件。情感粗粒度为积极情感和消极情感，细粒度为喜欢、厌恶、快乐、恐惧、惊讶、愤怒、悲伤七种。

 我们现在想的做法思路是使用词袋模型，然后提取特征，再构建分类器。

## 预测天猫用户下月的购买情况

### 成员

- 2120131028蒋浩浩 
- 2120141070薛景 
- 2120141071闫文真

## 

贾凌云 2120141014
 贾娜娜 2120141015
  付文飞2120141002

## 

汪洋 2120141052
冯伟 2120141001
张灿 2120141078