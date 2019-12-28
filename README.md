CCF Countdown
===

Countdown timers to keep track of deadlines of conferences recommended by [China Computer Federation (CCF)](https://www.ccf.org.cn/xspj/gyml/).

Based on [ai-deadlines](https://aideadlin.es/) by [@abshkdz](https://github.com/abhshkdz).

### Adding/updating a conference

To keep things minimal, I'm only looking to list CCF conferences. Feel free to maintain a separate fork if you don't see your sub-field or conference of interest listed.

To add or update information:
- Fork the repository
- Update `_data/conferences.yml`
- Make sure it has the `title`, `year`, `id`, `link`, `deadline`, `timezone`, `date`, `place`, `sub`, `rank` attributes
    + See available timezone strings [here](https://momentjs.com/timezone/).
- Optionally add a `note` and `abstract_deadline` in case the conference has a separate mandatory abstract deadline
- [Testing the GitHub Pages site locally with Jekyll](https://help.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll) if you want
- Send a pull request

### Conference entry record

Example record:

```
- title: ICDCS
  year: 2020
  id: icdcs20
  description: IEEE International Conference on Distributed Computing Systems
  link: https://icdcs2020.sg/
  deadline: '2020-01-13 23:59:59'
  abstract_deadline: '2020-01-06 23:59:59'
  timezone: UTC-7
  date: July 8-10, 2020
  place: Singapore
  sub: DS
  rank: B
```

Description of the fields:

| Field name          | Description                                                                      |
| ------------------- | -------------------------------------------------------------------------------- |
| `title`\*           | Short conference name, without year                                              |
| `year`\*            | Year the conference is happening                                                 |
| `description`\*     | Description, or long name                                                        |
| `id`\*              | Identifier of the conference                                                     |
| `link`\*            | URL to the conference home page                                                  |
| `deadline`\*        | Deadline                                                                         |
| `abstract_deadline` | Abstract deadline if applicable                                                  |
| `timezone`\*        | Timezone of the place where the conference is happening                          |
| `date`\*            | When the conference is happening                                                 |
| `place`\*           | Where the conference is happening                                                |
| `sub`\*             | The category that the conference is labeled by CCF, see the matching table below |
| `rank`\*            | The level that the conference is ranked by CCF, i.e., `A`, `B`, `C`              |
| `note`              | Some comments on the conference                                                  |

The matching table:

| Category name in [CCF](https://www.ccf.org.cn/xspj/gyml/) | `sub` field |
| --------------------------------------------------------- | ----------- |
| `计算机体系结构/并行与分布计算/存储系统`                  | `DS`        |
| `计算机网络`                                              | `NW`        |
| `网络与信息安全`                                          | `SC`        |
| `软件工程/系统软件/程序设计语言`                          | `SE`        |
| `数据库/数据挖掘/内容检索`                                | `DB`        |
| `计算机科学理论`                                          | `CT`        |
| `计算机图形学与多媒体`                                    | `CG`        |
| `人工智能`                                                | `AI`        |
| `人机交互与普适计算`                                      | `HI`        |
| `交叉/综合/新兴`                                          | `NEW`       |

### License

[MIT][1]
