# IELTS CD Practice 题库

[IELTS CD Practice](https://github.com/Gordonynh/ielts-cd-practice)（iPad 雅思机考练习 App）使用的题库。App 的安装脚本会自动下载本仓库，一般不需要手动操作。

## 内容

| 类别 | 数量 |
| --- | --- |
| 阅读 | 72 套 · 216 篇（剑桥雅思 5–21、红皮密卷，学术类） |
| 听力 | 72 套 · 288 个 Part |
| 写作 | 136 道题（48 篇附范文） |
| 机经 | 听力 128、阅读 60、写作 215 |
| 考试回忆 | 152 场（2025-11 – 2026-08） |
| 口语 | 100 个话题 · 658 道题 |

```text
bank/
  index.json                         阅读篇目、整套试卷、听力试卷、写作题目索引
  reading/exams/<id>.json            阅读（每篇一个文件，id = <套题 id>-p<Part>）
  reading/explanations/<id>.json     阅读解析与段落翻译
  listening/exams/<id>.json          听力（每个 Part 一个文件，id = <套题 id>-l<Part>）
  listening/explanations/<id>.json   听力解析与原文
  extras.json                        机经、考试回忆、写作题目、口语题库
  images/                            题目插图
```

- **听力音频**：不在本仓库。App 按题目里记录的原发布地址在线播放，也可以在 App 中按套下载。
- **段落翻译**：部分阅读的段落翻译由 Apple 翻译机器生成，可能有不准确之处。
- **生成方式**：文件由 App 仓库的 `scripts/build-bank.mjs` 与 `scripts/build-extras.mjs` 生成，源文件格式见 App 仓库的 `docs/题库数据格式.md`。

## 手动安装

不使用安装脚本时，把 `bank/` 复制到 App 仓库的 `IELTSCDPractice/Content/bank/`，再编译 App 即可。

## 授权与版权

- **使用范围**：请仅用于个人学习与备考。转载或用于其他用途前，请先确认符合权利人的授权范围。
- **联系**：如有版权问题，请提 [Issue](https://github.com/Gordonynh/ielts-cd-practice-content/issues) 联系，收到后会及时处理。
- **商标**：IELTS 是其所有者的注册商标。
