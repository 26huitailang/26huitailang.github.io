---
layout: post
title: 还是决定投靠Anaconda
date: 2016-08-05
tagline: 告别手动
---

当我被安装包的各种兼容耗费了许久之后，还是决定投靠anaconda的怀抱，发现已经更新到了anaconda2，而且安装之后泪流满面，输入conda list之后，简直泪流满面，除了个别包，基本和用过的是重叠，甚至还有许多学习数据分析的过程中会用到的其他基础包。  

### 被scipy和seaborn逼走了

用了一上午的时间还没有解决这中间发生的问题，碰巧前几天刚好看了anaconda的详细介绍，所以决定动手试试，是时候告别手动时代，及时有requirements.txt这种可维护的东西，但还是免不了各种折腾，anaconda对于我这样的初学者机会就是一步到位。

1. 下载安装相应的anaconda版本，双击安装，然后可以使用conda list查看已有的包，有其他需要可以再补上
2. 这里说明一下大家都可能遇到的问题，在import seaborn时会提示_cannot import name NUMPY_MKL_，这是因为pip install numpy导致没有mkl，所以应该去下载相应的.whl文件，[地址在这里](http://www.lfd.uci.edu/~gohlke/pythonlibs/#numpy)。
3. 下载好后，把whl文件放到需要安装的python环境\Scripts下，用pip install xxx.whl安装，默认会卸载相应环境的numpy并安装新的numpy+mkl。
4. 搞定！

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```

And flow charts like this:

```flow
st=>start: Start
e=>end
op=>operation: My Operation
cond=>condition: Yes or No?

st->op->cond
cond(yes)->e
cond(no)->op
```

> **Note:** You can find more information:

> - about **Sequence diagrams** syntax [here][7],
> - about **Flow charts** syntax [here][8].

### Support StackEdit

[![](https://cdn.monetizejs.com/resources/button-32.png)](https://monetizejs.com/authorize?client_id=ESTHdCYOi18iLhhO&summary=true)

  [^stackedit]: [StackEdit](https://stackedit.io/) is a full-featured, open-source Markdown editor based on PageDown, the Markdown library used by Stack Overflow and the other Stack Exchange sites.


  [1]: http://math.stackexchange.com/
  [2]: http://daringfireball.net/projects/markdown/syntax "Markdown"
  [3]: https://github.com/jmcmanus/pagedown-extra "Pagedown Extra"
  [4]: http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference
  [5]: https://code.google.com/p/google-code-prettify/
  [6]: http://highlightjs.org/
  [7]: http://bramp.github.io/js-sequence-diagrams/
  [8]: http://adrai.github.io/flowchart.js/
