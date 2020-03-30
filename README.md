# Acemap汇总新型冠状病毒疫情数据仓库

在此仅分享原始数据，相关数据处理后的信息和解决方案以及呈现形式请参考以下内容：

- [ncp-acemap数据分析平台](http://ncp.acemap.info/)
- [浅析新冠病毒如何利用迁徙轨迹攻击人类](https://mp.weixin.qq.com/s/5y_1bRryI59zAPo1KYNpZA)
- [看新冠病毒的笼罩下，我们是如何反击的](https://mp.weixin.qq.com/s/oH2y0WPACDkAWQQhznsHqw)
- [面对新冠病毒，用知识图谱助力早发现早报告](https://mp.weixin.qq.com/s/SHiWPu5UZqMVQbPsb3p5dw)

## *所有的数据均是截止于2020年3月28日*我们将会定期进行更新和补充

## paper data

- **paper**文件夹中有所有ncov相关论文的解析后的数据，比Kaggle上面的一个比赛数据还要丰富。
- **paper/ncov_paper.xlsx**存放了每篇文章的明细

---

## 国际病例信息

    international_record.csv

- A：date 日期
- B：location ID 当地编号
- E：Country Name 国家名称
- F： Country English Name 国家英文名称
- G：Province Name 省名
- H：Province Short Name 省名简称
- I：Province English Name 省区英文名
- J：Current Confirmed Count 现在确认病例数
- K：Confirmed Count 确诊病例总数
- L：Suspected Count 疑似病例数
- M：Cured Count 已治愈病例数
- N：Dead Count 死亡病例数
- P：Update Time 更新时间

---

## 城市病例信息

    city_record.csv

- A: date 日期
- B: city name 城市名
- C: city English name 城市英文名
- D: current confirmed count 现在确诊数
- E: confirmed count 确诊总数
- F: suspected count 疑似病例数
- G: cured count 治愈病例数
- H: dead count 死亡病例数
- I: local ID 当地编号

---

## 省份病例信息

    province_record.csv

- date 日期
- local ID 当地编号
- continent name 洲名
- continent English name 洲英文名
- country name 国家名
- country English name 国家英文名
- province name 省名
- province short name 省简称
- province English name 省英文名
- current confirmed count 目前确认病例数
- confirmed count 确诊病例数
- suspected count 疑似病例数
- cured count 治愈病例数
- dead count 死亡病例数
- comment 备注
- update time 更新时间

---

## 武汉迁徙指数

    wuhan_migration_new

- city 目标城市
- date 日期
- rate  武汉每日迁出至各市的详细数量（规模指数 $*$ 比例 $*$ 100）

---

## 确诊患者的相关轨迹信息

    raw_traces.csv

- 位置
- 发布时间
- 病患信息
- 其他信息
- 行为轨迹(是个字典，可使用LDA主题分析进行文本分析)
- 来源

---

## 本数据仓库数据整理贡献者

- **组长**
  - 邓程 [[Github](https://github.com/davendw49/)] [[Email](mailto:davendw@sjtu.edu.cn)]

- **疫情数字与新闻数据**

  - 张逸晗 [[Github](https://github.com/tilendlesa/)] [[Email](mailto:1902942521@qq.com)]
  - 刘子卉 [[Email](mailto:zihui_liu@sjtu.edu.cn)]
  - 彭峰 [[Github](https://github.com/PFpengfeng/)] [[Email](mailto:2350212276@sjtu.edu.cn)]
  - 徐奕 [[Github](https://github.com/Reacubeth/)] [[Email](mailto:davendw@sjtu.edu.cn)]

- **论文数据**

  - 任雨阳 [[Email](mailto:yyren@tju.edu.cn)]
  - 宋昀翀 [[Github](https://github.com/Cyberpuncrush/)] [[Email](mailto:songyunchong@outlook.com
)]
  - 佟博 [[Github](https://github.com/iiot-tbb/)] [[Email](mailto:bool_tbb@sjtu.edu.cn)]
  - 韩周 [[Email](mailto:uptome@sjtu.edu.cn)]
