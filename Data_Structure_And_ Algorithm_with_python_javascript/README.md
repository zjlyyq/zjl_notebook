<p align="center">
    <img src="https://user-images.githubusercontent.com/19553554/71825144-2d568180-30d6-11ea-8ee0-63c849cfd934.png" alt="pyecharts logo" width=200 height=200 />
</p>
<h1 align="center">pyecharts</h1>
<p align="center">
    <em>Python ❤️ Echarts = pyecharts</em>
</p>
<p align="center">
    <a href="https://travis-ci.org/pyecharts/pyecharts">
        <img src="https://travis-ci.org/pyecharts/pyecharts.svg?branch=master" alt="Travis Build Status">
    </a>
    <a href="https://ci.appveyor.com/project/chenjiandongx/pyecharts">
        <img src="https://ci.appveyor.com/api/projects/status/81cbsfjpfryv1cl8/branch/master?svg=true" alt="Appveyor Build Status">
    </a>
    <a href="https://codecov.io/gh/pyecharts/pyecharts">
        <img src="https://codecov.io/gh/pyecharts/pyecharts/branch/master/graph/badge.svg" alt="Codecov">
    </a>
    <a href="https://badge.fury.io/py/pyecharts">
        <img src="https://badge.fury.io/py/pyecharts.svg" alt="Package version">
    </a>
    <a href="https://pypi.org/project/pyecharts/">
        <img src="https://img.shields.io/pypi/pyversions/pyecharts.svg?colorB=brightgreen" alt="PyPI - Python Version">
    </a>
</p>
<p align="center">
    <a href="https://pypi.org/project/pyecharts">
        <img src="https://img.shields.io/pypi/format/pyecharts.svg" alt="PyPI - Format">
    </a>
     <a href="https://github.com/pyecharts/pyecharts/pulls">
        <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat" alt="Contributions welcome">
    </a>
    <a href="https://opensource.org/licenses/MIT">
        <img src="https://img.shields.io/badge/License-MIT-brightgreen.svg" alt="License">
    </a>
</p>

本项目主要是用python和JavaScript实现常见的数据结构和算法。一方面是学习常用的数据结构和算法，另一方面是提高python和js的熟练度。
### 字符串匹配
#### BF算法（Bryte Force）
又称暴力匹配算法。主串长度为n，子串长度为m（n>m）。算法负责度为O(n*m)。
#### Rk算法（Rabin-Karp）
哈希算法对主串中的 n-m+1 个子串分别求哈希值，然后逐个与模式串的哈希值比较大小。如果某个子串的哈希值与模式串相等，那就说明对应的子串和模式串匹配了（这里先不考虑哈希冲突的问题，后面我们会讲到）。因为哈希值是一个数字，数字之间比较是否相等是非常快速的，所以模式串和子串比较的效率就提高了。
> 这个算法的关键在于哈希算法要设计的好，既方便运算有能降低哈希冲突的概率

#### BM算法（Boyer-Moore）
“坏字符规则”和“好前缀规则”