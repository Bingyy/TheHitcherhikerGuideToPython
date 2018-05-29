### 先上几条命令：

```bash
pip3 install pep8 # 快过时了
pip3 install pycodestyle # 取代上面这条
pip3 install autopep8
```

前两条用于代码审查，使用方式是：

```bash
pycodestyle UI.py
```

就会自动给出评价，看是否符合PEP8的风格规范。

那我们肯定在想，只给出诊断，是不是还要自己动手一点点改呢？答案是不用的。这也是`autopep8`的作用。

```bash
autopep8 UI.py
```

这样做的话，会直接在终端弹出修改过的代码，但是不会体现在代码文件里。

```bash
autopep8 --in-place UI.py
```

这样即可以直接在文件中修改代码风格。

`--in-place`可以配合`--aggressive`使用，后者表示改变的会很激进，这个选项甚至会修改非空白字符。

对于一个终端命令的使用，`autopep8 -h`查看帮助文件，稍稍认真读一下，再加上一点点的试验测试，基本就可以掌握了，这是比较官方的靠谱的做法。