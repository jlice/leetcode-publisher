## leetcode-publisher

Automatically generate and publish LeetCode solution repository.

Example: [My accepted leetcode solutions](https://github.com/jlice/leetcode)

<p align="center"><img src="https://user-images.githubusercontent.com/9983385/55671789-3bb50a00-58c6-11e9-9296-38c2e98df4cc.gif"></p>

### Instructions

1. Download this tool

```Bash
$ git clone https://github.com/jlice/leetcode-publisher.git
```

2. Install dependencies (requires Python 3.5 or higher)

```Bash
$ cd leetcode-publisher
$ pip install -r requirements.txt
```

3. Configure (copy `config.example.yml` to `config.yml` and edit it)

```Bash
$ cp config.example.yml config.yml
$ vim config.yml
```

4. Enjoy it!

```Bash
$ python src/app.py
```

### Description

This tool will automatically retrieve your data on LeetCode and cache it in the `_cache` folder so you don't need to retrieve data from LeetCode repeatedly.

The solution repository is generated in the `repo` folder, which is deleted before each build. The contents of the `_source` folder will be copied to the `repo` folder when the repository is generated.

The templates for the README and the solution are written in [Jinja2](http://jinja.pocoo.org/) and located in the `templ` folder.

Only get and display accepted codes. If codes in the same programming language are accepted multiple times, only the latest ones are displayed. If multiple programming languages are used to answer questions, answers in multiple programming languages will be presented.

### Agreement

[The MIT License](LICENSE)
