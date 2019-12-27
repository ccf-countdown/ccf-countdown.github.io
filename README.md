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
  link: https://icdcs2020.sg/
  deadline: '2020-01-13 23:59:59'
  abstract_deadline: '2020-01-06 23:59:59'
  timezone: UTC-7
  date: July 8-10, 2020
  place: Singapore
  sub: DS
  rank: B
```

### License

[MIT][1]
