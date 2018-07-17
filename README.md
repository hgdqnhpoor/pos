# pos-
###正则
#正则导读
1. 正则是匹配模式，要么匹配字符，要么匹配位置
2. 在正则可以使用括号捕获数据，要么在API中进行分组引用，要么在正则里进行反向引用
3. 学习正则是需要了解其匹配原理的
4. 讲解正则表达式的回溯法原理
5. 从读的角度，去拆分一个正则表达式
6. 从写的角度，去构建一个正则表达式，也讲解了正则的表达式的整体工作流程
7. 讲解了正则的用法，和相关API需要注意的地方

#1.第一章  正则表达式字符匹配攻略

*正则表达式是匹配模式，要么匹配字符，要么匹配位置。*

内容包括:
- 两种模糊匹配
- 字符串
- 量词
- 分支结构
- 案例分析
##1.1. 两种模糊匹配
*如果正则只有精确匹配是没多大意义的,比如/hello/,也只能匹配字符串中的“hello”这个子串*
``
 var regex=/hello/;
 console.log(regex.test("hello"));

``
*正则表达式之所以强大,是因为其能实现模糊匹配*
*而模糊匹配，有两个方向上的“模糊”:横向模糊和纵向模糊*

