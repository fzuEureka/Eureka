#**A计划_阶段1**




[TOC]





#1.数据结构

【1】树状数组：成段修改，区间最大值，前缀最大值

【2】主席树

1.http://www.lydsy.com/JudgeOnline/problem.php?id=3932

2.http://codeforces.com/contest/787/problem/E

3.http://codeforces.com/contest/588/problem/E

4.http://codeforces.com/contest/707/problem/D

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3956

6.http://www.lydsy.com/JudgeOnline/problem.php?id=2006

7.http://www.lydsy.com/JudgeOnline/problem.php?id=4448

8.http://codeforces.com/problemset/problem/916/D

9.http://codeforces.com/problemset/problem/484/E

注：二分+可持久化线段树，离线从大到小插入权值，维护01串，查询区间最长"1"段的长度，典型的三段论线段树

特别注意：merge函数，不要把参数设置成const node &p形式，让其自然的拷贝，

避免x=merge(x,y)中x自更新不完全导致的错误

10.https://www.lydsy.com/JudgeOnline/problem.php?id=5494

11.https://www.lydsy.com/JudgeOnline/problem.php?id=5361





【3】树链剖分

指定题目：

1.http://www.lydsy.com/JudgeOnline/problem.php?id=4034

https://www.cnblogs.com/skylee03/p/8066974.html#commentform

树剖做法比其他两个多了log，但是比较通用。其他两个暂时还不知道有啥用。

2.http://www.lydsy.com/JudgeOnline/problem.php?id=3626

3.http://www.lydsy.com/JudgeOnline/problem.php?id=3531

4.http://www.lydsy.com/JudgeOnline/problem.php?id=2243

5.http://www.lydsy.com/JudgeOnline/problem.php?id=2543

6.https://www.lydsy.com/JudgeOnline/problem.php?id=1146

7.https://www.lydsy.com/JudgeOnline/problem.php?id=4712

8.https://www.lydsy.com/JudgeOnline/problem.php?id=3083

9.https://www.lydsy.com/JudgeOnline/problem.php?id=5210

10.http://clatisus.com/Discover%20Vladivostok%202018%20day%202#i.-kindom-and-roads

11.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=010435 A






【4】动态树lct

先看论文：https://wenku.baidu.com/view/7857b870aaea998fcc220ed8.html

指定题目：

1.http://www.lydsy.com/JudgeOnline/problem.php?id=1036

2.http://www.lydsy.com/JudgeOnline/problem.php?id=2002

3.http://www.lydsy.com/JudgeOnline/problem.php?id=2759

4.http://www.lydsy.com/JudgeOnline/problem.php?id=4012

**解法一：**

点分治可以查询块内的点与当前重心的信息，点分树是将这个信息减去重复统计的。

通常先把点分树建出来，然后像点分治那样正常统计。

统计的细节稍微推一下。

**解法二：**

dis(a, b) = dis(a) + dis(b) - 2 * dis(lca(a, b))

离线：和bzoj3626差不多。线段树的部分可以标记不下传。

在线：用主席树。

5.http://codeforces.com/contest/482/problem/E

6.http://www.lydsy.com/JudgeOnline/problem.php?id=2049

7.http://www.lydsy.com/JudgeOnline/problem.php?id=3669

8.http://www.lydsy.com/JudgeOnline/problem.php?id=4025

`3` `20190607` `bzoj4025` `LCT` `线段树分治` `可撤销并查集`

9.http://www.lydsy.com/JudgeOnline/problem.php?id=2843

10.http://www.lydsy.com/JudgeOnline/problem.php?id=2959

11.http://acm.hdu.edu.cn/showproblem.php?pid=5002

12.http://acm.hdu.edu.cn/showproblem.php?pid=4836

13.http://acm.hdu.edu.cn/showproblem.php?pid=5314

14.http://acm.hdu.edu.cn/showproblem.php?pid=5398

15.http://acm.hdu.edu.cn/showproblem.php?pid=4677

16.http://acm.hdu.edu.cn/showproblem.php?pid=4010

17.http://uoj.ac/problem/207

18.http://acm.hdu.edu.cn/showproblem.php?pid=6394

19.https://www.lydsy.com/JudgeOnline/problem.php?id=4229

20.https://www.lydsy.com/JudgeOnline/problem.php?id=1969

21.https://www.lydsy.com/JudgeOnline/problem.php?id=4530

22.https://www.lydsy.com/JudgeOnline/problem.php?id=2631

23.https://www.lydsy.com/JudgeOnline/problem.php?id=3091

24.https://www.lydsy.com/JudgeOnline/problem.php?id=4668

25.https://www.lydsy.com/JudgeOnline/problem.php?id=3282

26.https://www.lydsy.com/JudgeOnline/problem.php?id=4998

27.https://www.lydsy.com/JudgeOnline/problem.php?id=3159

28.https://www.lydsy.com/JudgeOnline/problem.php?id=2555

29.https://www.lydsy.com/JudgeOnline/problem.php?id=5212

30.https://www.lydsy.com/JudgeOnline/problem.php?id=3510

31.https://www.lydsy.com/JudgeOnline/problem.php?id=4736

或者：http://uoj.ac/problem/274

32.https://www.lydsy.com/JudgeOnline/problem.php?id=3639

33.https://www.lydsy.com/JudgeOnline/problem.php?id=3514

34.https://www.lydsy.com/JudgeOnline/problem.php?id=5048

35.https://www.lydsy.com/JudgeOnline/problem.php?id=2001

36.https://www.lydsy.com/JudgeOnline/problem.php?id=5379

37.https://www.lydsy.com/JudgeOnline/problem.php?id=4817

38.https://www.lydsy.com/JudgeOnline/problem.php?id=2594

39.https://www.lydsy.com/JudgeOnline/problem.php?id=2594

40.https://www.lydsy.com/JudgeOnline/problem.php?id=2836

41.https://www.lydsy.com/JudgeOnline/problem.php?id=4764

42.https://www.lydsy.com/JudgeOnline/problem.php?id=3779

43.http://codeforces.com/problemset/problem/891/C

44.http://codeforces.com/problemset/problem/603/E

45.https://www.lydsy.com/JudgeOnline/problem.php?id=5192

`3` `20190615` `bzoj5912` `点分树` `动态点分治` `树直径`












【5】SBT/treap旋转版本

注意：了解只是说不要求掌握到很深的程度，但是不代表不看不学  

   最好找点零碎的时间，一点点学掉，不需要做很多题目

   


【6】斜堆/左偏树







【7】可持久化数据结构与启发式合并学习



1）利用熟练剖分或者动态树套主席树，来复习主席树，学习标记永久化，历史最值问题（看论文）

1.BZOJ 1513

2.http://www.lydsy.com/JudgeOnline/problem.php?id=3110

3.http://poj.org/problem?id=2155

历史最值与区间最值操作

1.http://www.lydsy.com/JudgeOnline/problem.php?id=3064

2.http://acm.hdu.edu.cn/showproblem.php?pid=5306

3.http://uoj.ac/problem/164

4.http://www.tyvj.cn/p/1518

5.http://uoj.ac/problem/25

6.http://uoj.ac/problem/169

7.http://blog.csdn.net/s_g_g/article/details/53065776



2）学习可持久化并查集/带撤销与回滚功能的并查集/可持久化数组，与一些重要的应用

1.http://www.lydsy.com/JudgeOnline/problem.php?id=3674

2.http://www.lydsy.com/JudgeOnline/problem.php?id=3673

3.http://acm.hdu.edu.cn/showproblem.php?pid=5923

4.https://uva.onlinejudge.org/index.php?option=com_onlinejudge&Itemid=8&category=229&page=show_problem&problem=3138

5.http://codeforces.com/contest/892/problem/E




3）学习非旋转版本的treap,与启发式合并，以及如何可持久化treap

1.https://uva.onlinejudge.org/index.php?option=com_onlinejudge&Itemid=8&category=441&page=show_problem&problem=3983

2.http://codeforces.com/problemset/problem/702/F

3.http://codeforces.com/group/aUVPeyEnI2/contest/243687 L题

注：维护序列切割经典题





4）可持久化队列

http://www.cnblogs.com/qscqesze/p/4738165.html





5）可持久化字典树

1.http://www.lydsy.com/JudgeOnline/problem.php?id=2741

2.http://blog.csdn.net/u014609452/article/details/51416634

3.http://blog.csdn.net/u014609452/article/details/51416605

4.http://acm.hdu.edu.cn/showproblem.php?pid=4757

5.http://codeforces.com/problemset/problem/916/D



6）可持久化块状链表




7）启发式合并

并查集
1.http://codeforces.com/contest/778/problem/C

伸展树
2.http://www.lydsy.com/JudgeOnline/problem.php?id=2809

链表
3.http://www.lydsy.com/JudgeOnline/problem.php?id=1483

treap
4.http://www.lydsy.com/JudgeOnline/problem.php?id=2733

treap
5.http://poj.org/problem?id=1471

map
6.http://acm.uestc.edu.cn/#/problem/show/1284

LCT
7.http://www.cnblogs.com/geng4512/p/5296855.html

主席树
8.http://www.lydsy.com/JudgeOnline/problem.php?id=3123

set
9.http://bestcoder.hdu.edu.cn/contests/contest_showproblem.php?cid=775&pid=1002

10.http://codeforces.com/contest/375/problem/D

线段树

https://wenku.baidu.com/view/88f4e134e518964bcf847c95.html

11.http://codeforces.com/contest/893/problem/F

12.http://www.lydsy.com/JudgeOnline/problem.php?id=4552

13.https://nanti.jisuanke.com/t/30997

【8】树上分治算法

1）点分治

1.http://poj.org/problem?id=1741

2.http://acm.hdu.edu.cn/showproblem.php?pid=4812

3.http://codeforces.com/contest/161/problem/D

4.http://www.lydsy.com/JudgeOnline/problem.php?id=3697

5.http://www.lydsy.com/JudgeOnline/problem.php?id=2152

6.http://www.lydsy.com/JudgeOnline/problem.php?id=3648

7.http://www.lydsy.com/JudgeOnline/problem.php?id=3784

`3` `20190605` `bzoj3784` `点分治` `思维`

解法一：二分下界。可以先把sort过的数组存起来优化复杂度。

解法二：转化成 `bzoj2006` 做。

解法二会好写点。

8.http://www.lydsy.com/JudgeOnline/problem.php?id=1095

9.http://uoj.ac/problem/33

10.http://www.spoj.com/problems/FTOUR2/

11.http://www.lydsy.com/JudgeOnline/problem.php?id=4016

`3` `20190606` `bzoj4016` `点分治` `最短路径树`

12.http://www.lydsy.com/JudgeOnline/problem.php?id=1758

13.http://www.lydsy.com/JudgeOnline/problem.php?id=2599

14.http://www.lydsy.com/JudgeOnline/problem.php?id=1468

15.http://poj.org/problem?id=1987

16.http://www.lydsy.com/JudgeOnline/problem.php?id=3730

17.http://www.lydsy.com/JudgeOnline/problem.php?id=3365

18.http://www.lydsy.com/JudgeOnline/problem.php?id=1316

19.http://www.lydsy.com/JudgeOnline/problem.php?id=2006

20.http://www.lydsy.com/JudgeOnline/problem.php?id=3451

21.http://www.spoj.com/problems/QTREE5/

22.https://cn.vjudge.net/contest/187749#problem/G

23.http://codeforces.com/problemset/problem/914/E

24.http://codeforces.com/problemset/problem/960/E

25.https://codeforces.com/problemset/problem/1019/E

2）边分治

1.http://www.lydsy.com/JudgeOnline/problem.php?id=5152

2.http://www.lydsy.com/JudgeOnline/problem.php?id=5341

3）动态点分治

1.https://www.lydsy.com/JudgeOnline/problem.php?id=4372

`2` `20190610` `bzoj4372` `点分树` `线段树`

2.https://www.lydsy.com/JudgeOnline/problem.php?id=5192

`3` `20190615` `bzoj5912` `点分树` `动态点分治` `树直径`



【9】动态树问题的几个扩展与经典应用

1）EET

2）Top Tree

【10】各类树套树与动态经典问题

1）线段树套平衡树

1.http://blog.csdn.net/u014609452/article/details/51428431

2.http://www.lydsy.com/JudgeOnline/problem.php?id=3196

3.http://www.lydsy.com/JudgeOnline/problem.php?id=2141

4.http://www.cnblogs.com/iwtwiioi/p/3925416.html

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3295

6.http://www.lydsy.com/JudgeOnline/problem.php?id=1058

7.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2112

8.http://codeforces.com/problemset/problem/785/E

9.http://codeforces.com/problemset/problem/19/D

注：线段树维护一组set中最大值的变化，查询>=pos下标中值>=x的最小下标，在指定set中进一步维护或者查询

2）树状数组套主席树

1.http://www.lydsy.com/JudgeOnline/problem.php?id=2120

2.http://blog.csdn.net/clove_unique/article/details/54318285

3.http://www.lydsy.com/JudgeOnline/problem.php?id=3110

4.http://www.lydsy.com/JudgeOnline/problem.php?id=4785

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3932


3）动态仙人掌问题

4）动态凸包问题

【11】STL中的pd_bs库和rope大法

【12】kd-tree

1.http://www.lydsy.com/JudgeOnline/problem.php?id=4358

2.http://www.lydsy.com/JudgeOnline/problem.php?id=2683

3.http://www.lydsy.com/JudgeOnline/problem.php?id=4066

4.http://www.lydsy.com/JudgeOnline/problem.php?id=2850

5.http://www.lydsy.com/JudgeOnline/problem.php?id=2626

6.http://www.lydsy.com/JudgeOnline/problem.php?id=4520

7.http://www.lydsy.com/JudgeOnline/problem.php?id=2989

8.http://www.lydsy.com/JudgeOnline/problem.php?id=4130

9.http://www.lydsy.com/JudgeOnline/problem.php?id=2648

10.http://www.lydsy.com/JudgeOnline/problem.php?id=2716

11.http://www.lydsy.com/JudgeOnline/problem.php?id=3053

12.http://www.lydsy.com/JudgeOnline/problem.php?id=3489

13.http://www.lydsy.com/JudgeOnline/problem.php?id=4154

14.http://www.lydsy.com/JudgeOnline/problem.php?id=3007

15.http://www.lydsy.com/JudgeOnline/problem.php?id=4219

16.http://www.lydsy.com/JudgeOnline/problem.php?id=4605

17.http://acm.hdu.edu.cn/showproblem.php?pid=2966

18.http://acm.hdu.edu.cn/showproblem.php?pid=4347

19.http://acm.hdu.edu.cn/showproblem.php?pid=5992

20.http://www.lydsy.com/JudgeOnline/problem.php?id=1941

21.https://nanti.jisuanke.com/t/31451




【13】veb树（van Emde Boas）

1.https://www.lydsy.com/JudgeOnline/problem.php?id=3685



【14】基础数据结构经典题

不交区间并set：

1.http://codeforces.com/problemset/problem/915/E

2.http://codeforces.com/problemset/problem/915/F

3.http://codeforces.com/problemset/problem/926/J

离散化线段树：

1.http://codeforces.com/problemset/problem/817/F

线段树+自然hash+递归开关:

1.http://codeforces.com/problemset/problem/914/D

优先队列+全局非负减/全局标记：

1.http://codeforces.com/problemset/problem/923/B

2.https://vjudge.net/contest/274500#problem/K

二分+贪心+单调队列/双指针:

1.http://codeforces.com/problemset/problem/924/B

数形结合+逆序对：

1.http://codeforces.com/problemset/problem/924/D

字典树+贪心式处理：

1.http://codeforces.com/problemset/problem/928/D

动态地树上倍增：

1.http://codeforces.com/problemset/problem/932/D

优先队列模拟题：

1.http://codeforces.com/problemset/problem/962/D

线段树模拟费用流：

1.https://www.lydsy.com/JudgeOnline/problem.php?id=4977


线段树单点修改+查询pos右侧第一个大于/小于x的下标：
(维护区间最值，左子树合法时优先查询，有解直接返回，然后考虑右子树)

1.https://nanti.jisuanke.com/t/30996

无穷序列逆序对问题：

1.http://codeforces.com/problemset/problem/540/E

http://acm.hdu.edu.cn/showproblem.php?pid=6291


【15】数据结构中档题

1.http://codeforces.com/problemset/problem/961/E

2.https://nanti.jisuanke.com/t/31459

3.https://nanti.jisuanke.com/t/31460

4.https://nanti.jisuanke.com/t/31714

5.http://codeforces.com/problemset/problem/1000/F

6.http://codeforces.com/problemset/problem/1083/C

注：线段树合并式dp，一个节点[l,r]存储树上包含此闭区间数值的最小链端点对，此信息可单点修改，合并维护

查询最小非法前缀，查询时，带一个动态修改的查询参数，表示当前区间[l,r]严格前面的区间[0,l-1]的信息并

查询时，左子树不可并，递归去左子树，否则右子树；叶节点特判是否符合



【15】双指针

1.http://codeforces.com/problemset/problem/901/C

2.http://codeforces.com/problemset/problem/939/E

3.http://codeforces.com/problemset/problem/958/F2



【16】延迟操作/懒标记思想/相对运动懒标记/隐式删除/差分思想与前缀和/数学变换的表达与转化

1.http://codeforces.com/problemset/problem/924/C

2.http://codeforces.com/problemset/problem/960/D



【17】长链剖分

参考资料：

https://blog.bill.moe/long-chain-subdivision-notes/

https://www.cnblogs.com/zzqsblog/articles/6700133.html

http://www.cnblogs.com/zhoushuyu/p/9468669.html

https://www.cnblogs.com/meowww/p/6403515.html

https://zhuanlan.zhihu.com/p/25984772

题目：

1.https://vijos.org/d/Bashu_OIers/p/5a79a3e1d3d8a103be7e2b81

2.https://www.lydsy.com/JudgeOnline/problem.php?id=4543

`5` `20190610` `bzoj4543` `长链剖分` `dp`

- 前置题目 bzoj3522，其实没啥联系
- dp状态不好想
  - $g[u][i]$ 表示 u 的子树中有多少个 pair 对只要在 u 顶上加一条长度 i 的就凑成一个合法的三元组了
  - $f[u][i]$ 表示 u 的子树中有多少个点与 u 距离 i
  - dep[u] 表示 u 与子树中最远的叶子距离
  - 显然 i 的范围是 0 到 dep[u]
- 转移
  - 一棵子树一棵子树的加，考虑新加子树与原来那一坨对答案的贡献
  - 考虑子树中已有的 g 数组，新子树与原来一坨对当前 g 的贡献
  - f 比较简单
- 长链剖分
  - f 比较简单
  - g 的过程就是把最前面那个删掉，在最后面加上两个。首先要倒着存，其次数组开两倍。坐标重定位推一推。

3.https://www.lydsy.com/JudgeOnline/problem.php?id=1758

4.http://codeforces.com/problemset/problem/1009/F

5.https://www.lydsy.com/JudgeOnline/problem.php?id=3252

6.https://www.lydsy.com/JudgeOnline/problem.php?id=3653




【18】Leafy Tree 及其实现的加权平衡树

论文：2018年集训队论文


【19】基环树

1.http://codeforces.com/problemset/problem/875/F

求最大生成基环树，把二分图一边度都为2的点当成边是个套路 

2.https://www.lydsy.com/JudgeOnline/problem.php?id=1040

求基环树带权最大点独立集，注意自环和二元环时的重边 

3.https://www.lydsy.com/JudgeOnline/problem.php?id=3242

求边上一点到基环树最远点距离最小，可以转化成基环树断一条环边使直径最小

分类讨论，处理选的两点在断掉一边和分在两边的情况 

4.https://www.lydsy.com/JudgeOnline/problem.php?id=1791

求基环树的直径

5.https://www.lydsy.com/JudgeOnline/problem.php?id=2791

类似于基环树上求lca，分类讨论，注意自环 

6.https://www.lydsy.com/JudgeOnline/problem.php?id=2878

求基环树上任意起点走的路径长度期望，比较复杂的dp，以及常见的树上换根套路，环比较小，环上可以暴力做

7.https://www.lydsy.com/JudgeOnline/problem.php?id=1116

判断图是否有子图是基环树，水题，可以认为边权为1求最大生成基环树

8.http://acm.hdu.edu.cn/showproblem.php?pid=6370

9.http://acm.hdu.edu.cn/showproblem.php?pid=6403

10.http://acm.hdu.edu.cn/showproblem.php?pid=5304

11.http://acm.hdu.edu.cn/showproblem.php?pid=6393

12.http://acm.hdu.edu.cn/showproblem.php?pid=5967

13.https://agc008.contest.atcoder.jp/tasks/agc008_e

14.https://www.lydsy.com/JudgeOnline/problem.php?id=5362




【20】斯坦纳树

参考资料：

https://www.cnblogs.com/ECJTUACM-873284962/p/7643445.html

https://blog.csdn.net/wu_tongtong/article/details/78992913

论文：https://wenku.baidu.com/view/6b8f5c0102020740be1e9ba8.html

题目：

1.https://www.lydsy.com/JudgeOnline/problem.php?id=2959

2.https://www.lydsy.com/JudgeOnline/problem.php?id=3205

注：关键在建图，以及因为边权为1可以用多源bfs

3.https://www.lydsy.com/JudgeOnline/problem.php?id=4774

4.https://www.lydsy.com/JudgeOnline/problem.php?id=5180

注：如果图比较大且为正权，用dijstra 

5.https://www.lydsy.com/JudgeOnline/problem.php?id=4006

注：只要一些点对之间联通，做完斯坦纳树后再dp一遍 

6.http://codeforces.com/problemset/problem/152/E

注：要会记录方案

7.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3613

注：要注意如果一个点是两类关键点，设dp初值时状态要合起来

8.http://acm.hdu.edu.cn/showproblem.php?pid=3832

注：如果关键点小于等于3其实可以分别跑最短路枚举中间点算，不用斯坦纳树

9.http://acm.hdu.edu.cn/showproblem.php?pid=3311

注：点边都有代价，联通快中的点只要有一个付出代价就行，建超级源的技巧 ，向所有点连边权为点权的边

10.http://acm.hdu.edu.cn/showproblem.php?pid=4085

11.http://acm.csu.edu.cn/csuoj/problemset/problem?pid=1965





【21】虚树

1.https://www.lydsy.com/JudgeOnline/problem.php?id=3572

2.https://www.lydsy.com/JudgeOnline/problem.php?id=3991

`3` `20190605` `bzoj3991` `思维` `dfs序`

3.https://www.lydsy.com/JudgeOnline/problem.php?id=3611

4.https://www.lydsy.com/JudgeOnline/problem.php?id=2286

5.https://www.lydsy.com/JudgeOnline/problem.php?id=4912

`5` `20190615` `bzoj4912` `虚树` `前后缀优化建图` `dp`

6.https://www.lydsy.com/JudgeOnline/problem.php?id=3879

7.https://www.lydsy.com/JudgeOnline/problem.php?id=5287

8.https://www.lydsy.com/JudgeOnline/problem.php?id=5329

9.http://codeforces.com/problemset/problem/613/D

10.http://codeforces.com/problemset/problem/966/E

11.http://codeforces.com/problemset/problem/986/E

12.http://codeforces.com/problemset/problem/809/E

13.http://acm.hdu.edu.cn/showproblem.php?pid=6035

14.https://cn.vjudge.net/problem/CodeChef-BTREE

或者：https://www.codechef.com/problems/BTREE

15.http://codeforces.com/gym/102220/problem/D

注：一棵初始点权为0的树，树上链各种成段修改，建立虚树之后，注意到虚树上一小段的点权是一致的






【22】优化建图

## 线段树优化建图

### 题目

1.https://www.lydsy.com/JudgeOnline/problem.php?id=3073

2.https://www.lydsy.com/JudgeOnline/problem.php?id=4383

3.https://www.lydsy.com/JudgeOnline/problem.php?id=5017

4.http://codeforces.com/problemset/problem/786/B

5.http://acm.hdu.edu.cn/showproblem.php?pid=5669

6.http://uoj.ac/problem/77

7.https://arc069.contest.atcoder.jp/tasks/arc069_d

8.https://www.lydsy.com/JudgeOnline/problem.php?id=3218（与6重复）

9.https://www.lydsy.com/JudgeOnline/problem.php?id=4276

## 主席树优化建图

### 题目

https://www.lydsy.com/JudgeOnline/problem.php?id=3681

http://uoj.ac/problem/77

https://www.lydsy.com/JudgeOnline/problem.php?id=3218（与上一题是同一道）

https://www.luogu.org/problemnew/show/P5284

## 字典树优化建图

### 题目

https://www.luogu.org/problemnew/show/P5284

## 前后缀优化建图

### 题目

https://www.lydsy.com/JudgeOnline/problem.php?id=3495

https://www.lydsy.com/JudgeOnline/problem.php?id=4912

`5` `20190615` `bzoj4912` `虚树` `前后缀优化建图` `dp`

https://codeforces.com/problemset/problem/587/D

https://codeforces.com/problemset/problem/1007/D



【23】笛卡尔树

参考资料：

https://www.cnblogs.com/gtarcoder/p/4702853.html

https://blog.csdn.net/qq_15033645/article/details/80961472

http://www.cnblogs.com/CaptainSlow/p/9282507.html

https://blog.csdn.net/qq_36056315/article/details/79845193

https://en.wikipedia.org/wiki/Cartesian_tree#CITEREFSeidelAragon1996

题目：

1.http://acm.hdu.edu.cn/showproblem.php?pid=6305

2.http://acm.hdu.edu.cn/showproblem.php?pid=4095

3.http://acm.hdu.edu.cn/showproblem.php?pid=6044

4.http://acm.hdu.edu.cn/showproblem.php?pid=5324

5.http://acm.hdu.edu.cn/showproblem.php?pid=1506

6.http://acm.hdu.edu.cn/showproblem.php?pid=4125

7.http://acm.hdu.edu.cn/showproblem.php?pid=6406

8.http://acm.hdu.edu.cn/showproblem.php?pid=5412

9.https://www.lydsy.com/JudgeOnline/problem.php?id=2616

10.https://www.lydsy.com/JudgeOnline/problem.php?id=2658

11.http://poj.org/problem?id=1785

12.http://poj.org/problem?id=2201

13.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=010435 J



【24】李超树

【25】支配树

【26】高维偏序问题

【27】树上差分小专题

1.http://codeforces.com/gym/102012/problem/G


【28】曼哈顿距离和切比雪夫距离的转化

1.http://codeforces.com/problemset/problem/1093/G


【29】dsu on tree

1.http://codeforces.com/problemset/problem/600/E


【30】珂朵莉树

1.http://codeforces.com/problemset/problem/896/C

2.http://codeforces.com/problemset/problem/343/D

3.http://codeforces.com/problemset/problem/915/E

4.https://www.lydsy.com/JudgeOnline/problem.php?id=1858

5.https://www.lydsy.com/JudgeOnline/problem.php?id=4592

6.https://www.lydsy.com/JudgeOnline/problem.php?id=5168

7.https://www.luogu.org/problemnew/show/P2787

8.https://www.luogu.org/problemnew/show/P4979

9.https://www.luogu.org/problemnew/show/P1204











---



# 2.图论

##【1】差分约束系统（重点）

学习博客：http://www.cppblog.com/menjitianya/archive/2015/11/19/212292.html

注：

**理解**

在有向图最长路模型中，如果x到y存在一条权值和为c的有向路径，那么显然x到y的最长路不会小于c，那么即有dist[y]-dist[x]>=c，大于等于模型应该使用最长路

**关于解的存在性讨论**：

标准型形如x[i]-x[j]<=a[k]，j->i(边权a[k])，求$(x[t]-x[s])_{max}$(s到t最短路)

1)无解：s到t最短路为-oo，亦即a[t]-a[s]<=-oo显然无解；等价于图中存在s可以走到的负权环，用spfa某个点入队次数大于n来判定

2)无数解：s到t最短路为OO，即s根本走不到t，亦即a[t]-a[s]<=OO，若a[s]=0，a[t]可以任意取值

3)有限解：其余情况为有限解(假设某个变量取定值)

**关于简单建图**：

先看最后求的是什么，求$(x[t]-x[s])_{max}$，方向转化为<=，求最短路；

而如果求的是最小值，方向转化为>=，求最长路；

限制条件转化：

a=b转化为a>=b，a<=b

a < b在整数意义下，转化为a<=b-1

a + b >= c(常数)，转化为 a - (-b) >= c

**建图优化**

1).集合A连集合B，引中间点c

2).区间A连单点x，线段树优化建图

3).区间A连区间B，引中间点c，转化为2

**特别当心**

1).注意当形如a < b或者a > b的限制，如果a==b特判无解

2).注意题目中的隐藏条件：比如某个变量值必须为正数，源点dist[s]这个变量比如为0等

3).一个差分约束系统有解，则必有无穷多组解，当限制每个变量均>=c时，仍然有无穷解；

因此，任何图模型，等价于新增超级源点，连接每个点，边权为c





指定题目：

1.http://www.lydsy.com/JudgeOnline/problem.php?id=2330

2.http://acm.hdu.edu.cn/showproblem.php?pid=3666

3.http://acm.hdu.edu.cn/showproblem.php?pid=1531

4.http://acm.hdu.edu.cn/showproblem.php?pid=1534

5.http://codeforces.com/gym/100015/attachments G题

6.http://codeforces.com/problemset/problem/1131/D

7.http://codeforces.com/problemset/problem/241/E

8.https://www.lydsy.com/JudgeOnline/problem.php?id=4500

9.https://www.lydsy.com/JudgeOnline/problem.php?id=1202

10.https://www.lydsy.com/JudgeOnline/problem.php?id=4383

注：线段树优化建图+差分约束+拓扑排序思想

11.https://www.lydsy.com/JudgeOnline/problem.php?id=3436

12.https://www.lydsy.com/JudgeOnline/problem.php?id=3373

13.https://www.lydsy.com/JudgeOnline/problem.php?id=1731

14.https://www.lydsy.com/JudgeOnline/problem.php?id=2788

注：tarjan缩点+差分约束+floyed求最长路最小值

题目求最大值，建<=模型跑最短路，每个强连通分量，超级源点s连每个点边权为1；

dist[]求最大值，跑最短路是模型要求满足限制，求最大值是题目最大化的目标；

在此模型下，所有边权取负，转化为跑最长路求最小值

15.https://www.lydsy.com/JudgeOnline/problem.php?id=1077

注：floyed求任两个变量差的最大最小值，求最大值跑最长路，初值为最小值

16.https://www.lydsy.com/JudgeOnline/problem.php?id=3126

17.http://acm.hdu.edu.cn/showproblem.php?pid=6252

18.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2770

19.http://acm.hdu.edu.cn/showproblem.php?pid=1535

20.http://acm.hdu.edu.cn/showproblem.php?pid=1317

21.http://acm.hdu.edu.cn/showproblem.php?pid=4109

22.http://acm.hdu.edu.cn/showproblem.php?pid=1529

23.http://acm.hdu.edu.cn/showproblem.php?pid=3592

24.http://acm.hdu.edu.cn/showproblem.php?pid=4598

25.http://acm.hdu.edu.cn/showproblem.php?pid=1384

26.https://codeforces.com/gym/101611/problem/G





##【2】K短路问题/次小生成树（了解）

指定题目：

1.http://acm.hdu.edu.cn/showproblem.php?pid=2449

2.http://acm.hdu.edu.cn/showproblem.php?pid=4081

3.https://nanti.jisuanke.com/t/31445

##【3】度限制最小生成树/最优比率生成树/最小树形图（了解）

##【4】生成树的计数问题（了解）

1.http://codeforces.com/problemset/problem/156/D

##【5】Tarjan初步：

求割点/桥/最近公公祖先/强连通分支（重点）

求点双连通分量/边双连通分量（了解）

指定题目：

1.http://www.lydsy.com/JudgeOnline/problem.php?id=2438

2.http://www.lydsy.com/JudgeOnline/problem.php?id=2140

3.http://www.lydsy.com/JudgeOnline/problem.php?id=1194

4.http://codeforces.com/problemset/problem/639/F

5.http://codeforces.com/problemset/problem/962/F

6.https://www.lydsy.com/JudgeOnline/problem.php?id=5303

##【6】Kosaraju算法与缩点（重点）

##【7】Menger定理（了解）

##【8】传递闭包

##【9】图论基础综合题

1.http://codeforces.com/problemset/problem/864/F

2.http://codeforces.com/problemset/problem/919/D

3.http://codeforces.com/problemset/problem/845/G

4.http://codeforces.com/problemset/problem/949/C

5.https://nanti.jisuanke.com/t/31462

###【最短路综合】

1.http://codeforces.com/problemset/problem/938/D

2.https://nanti.jisuanke.com/t/31001

3.http://codeforces.com/problemset/problem/1070/A

4.https://codeforces.com/problemset/problem/843/D

[经典]动态最短路问题：

每次一条边权++，可以证明残差图上增量最短路取值有限，单次修改可以O(n+m)

残差图使得最短路满足可加性，意思是新增的一些边权使得最短路产生一个增量，此增量叠加到原来的最短路长度数组dist[]中即得到新图的最短路数组



###【欧拉图综合】

1.http://codeforces.com/problemset/problem/1152/E

注：欧拉路径方案构造



###【平面图和平面嵌入】

1.https://codeforces.com/gym/101611/problem/C

注：树的平面嵌入，坐标范围[1..1000000]*[1..20]



###【支配树/支配点】

1.http://codeforces.com/group/aUVPeyEnI2/contest/243687 H题

注：支配思想的应用



## 【10】一类边数很少的特殊图问题

https://www.lydsy.com/JudgeOnline/problem.php?id=5287

注：也可以用动态dp做

http://acm.hdu.edu.cn/showproblem.php?pid=5736



# 3.网络流

【1】最大流（最小割）（重点）

指定题目：

1.http://www.lydsy.com/JudgeOnline/problem.php?id=2229

2.http://www.lydsy.com/JudgeOnline/problem.php?id=1001

3.http://www.lydsy.com/JudgeOnline/problem.php?id=1797

4.http://www.lydsy.com/JudgeOnline/problem.php?id=2561

5.http://codeforces.com/problemset/problem/813/D

6.http://codeforces.com/problemset/problem/818/G

7.http://codeforces.com/problemset/problem/802/C

8.http://codeforces.com/problemset/problem/1082/G


【2】费用流/带负权环（重点）

指定题目：

1.http://www.lydsy.com/JudgeOnline/problem.php?id=1877

2.http://www.lydsy.com/JudgeOnline/problem.php?id=2668

3.http://www.lydsy.com/JudgeOnline/problem.php?id=2597

4.http://www.lydsy.com/JudgeOnline/problem.php?id=1834

【3】二分图最大匹配：匈牙利（了解）

【4】模型：最小点/边/路径覆盖/最大独立集/最小支配集（重点）

【5】模型：稳定婚姻系统（了解）

【6】带上下界的流（重点）

【7】最大团问题





【二分图综合】

不能评测的题目，一定要好好看题解

1.http://www.lydsy.com/JudgeOnline/problem.php?id=4205

2.https://www.byvoid.com/zhs/blog/noi-2009-transform

http://www.lydsy.com/JudgeOnline/problem.php?id=1562

3.http://www.lydsy.com/JudgeOnline/problem.php?id=1059

4.http://www.lydsy.com/JudgeOnline/problem.php?id=1191

5.http://www.lydsy.com/JudgeOnline/problem.php?id=1854

6.http://www.lydsy.com/JudgeOnline/problem.php?id=2150

7.http://www.lydsy.com/JudgeOnline/problem.php?id=1143

8.http://www.lydsy.com/JudgeOnline/problem.php?id=2744

9.http://www.lydsy.com/JudgeOnline/problem.php?id=2437

10.http://www.lydsy.com/JudgeOnline/problem.php?id=4443

11.http://www.lydsy.com/JudgeOnline/problem.php?id=4950

12.http://www.lydsy.com/JudgeOnline/problem.php?id=1433

13.http://www.lydsy.com/JudgeOnline/problem.php?id=3175

14.http://www.lydsy.com/JudgeOnline/problem.php?id=4554

15.http://www.lydsy.com/JudgeOnline/problem.php?id=4025

16.http://www.lydsy.com/JudgeOnline/problem.php?id=1934

17.http://www.lydsy.com/JudgeOnline/problem.php?id=2539

18.http://www.lydsy.com/JudgeOnline/problem.php?id=1189

19.http://www.lydsy.com/JudgeOnline/problem.php?id=3140

20.http://www.lydsy.com/JudgeOnline/problem.php?id=3291

21.http://www.lydsy.com/JudgeOnline/problem.php?id=1443

22.http://www.lydsy.com/JudgeOnline/problem.php?id=1475

23.http://www.lydsy.com/JudgeOnline/problem.php?id=1997

24.http://www.lydsy.com/JudgeOnline/problem.php?id=1741

25.http://www.lydsy.com/JudgeOnline/problem.php?id=4080

26.http://codeforces.com/group/aUVPeyEnI2/contest/243686 H题


【网络流综合】


建模阅读：https://wenku.baidu.com/view/a22336727fd5360cba1adb83.html
《最小割模型在信息学竞赛中的应用》

http://blog.csdn.net/qq_35649707/article/details/77482691


1.http://www.lydsy.com/JudgeOnline/problem.php?id=4514

2.http://www.lydsy.com/JudgeOnline/problem.php?id=1433

3.http://www.lydsy.com/JudgeOnline/problem.php?id=1934

4.http://www.lydsy.com/JudgeOnline/problem.php?id=1854

5.http://www.lydsy.com/JudgeOnline/problem.php?id=1834

6.http://www.lydsy.com/JudgeOnline/problem.php?id=1927

7.http://www.lydsy.com/JudgeOnline/problem.php?id=2673

8.http://www.lydsy.com/JudgeOnline/problem.php?id=3876

9.http://www.lydsy.com/JudgeOnline/problem.php?id=3698

10.http://www.lydsy.com/JudgeOnline/problem.php?id=2502

11.http://www.lydsy.com/JudgeOnline/problem.php?id=2055

12.http://poj.org/problem?id=2396

13.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3229

14.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2314

15.http://www.lydsy.com/JudgeOnline/problem.php?id=2406

16.http://www.lydsy.com/JudgeOnline/problem.php?id=3280

17.http://www.lydsy.com/JudgeOnline/problem.php?id=3112

18.http://www.lydsy.com/JudgeOnline/problem.php?id=1917

19.http://www.lydsy.com/JudgeOnline/problem.php?id=3218（此题有论文，好像是16或17年的）

http://blog.csdn.net/outer_form/article/details/50847581

20.http://www.lydsy.com/JudgeOnline/problem.php?id=1570

21.http://www.lydsy.com/JudgeOnline/problem.php?id=3532

22.http://www.lydsy.com/JudgeOnline/problem.php?id=3158

23.http://www.lydsy.com/JudgeOnline/problem.php?id=2561

24.http://www.lydsy.com/JudgeOnline/problem.php?id=1877

25.http://www.lydsy.com/JudgeOnline/problem.php?id=1412

26.http://www.lydsy.com/JudgeOnline/problem.php?id=3993

27.https://vjudge.net/contest/189299#problem/C

28.http://www.lydsy.com/JudgeOnline/problem.php?id=1070

29.http://www.lydsy.com/JudgeOnline/problem.php?id=1458

30.http://www.lydsy.com/JudgeOnline/problem.php?id=4823

31.http://www.lydsy.com/JudgeOnline/problem.php?id=1822

32.http://www.lydsy.com/JudgeOnline/problem.php?id=3681

33.http://www.lydsy.com/JudgeOnline/problem.php?id=1497

34.http://www.lydsy.com/JudgeOnline/problem.php?id=1266

35.http://www.lydsy.com/JudgeOnline/problem.php?id=1823

36.http://www.lydsy.com/JudgeOnline/problem.php?id=1823

37.http://www.lydsy.com/JudgeOnline/problem.php?id=1324

38.http://www.lydsy.com/JudgeOnline/problem.php?id=2095

39.http://acm.split.hdu.edu.cn/showproblem.php?pid=4807

40.https://vjudge.net/contest/189689#problem/I

41.http://hzwer.com/5844.html

42.http://hzwer.com/5842.html

43.http://hzwer.com/1955.html

44.http://hzwer.com/1758.html

45.http://www.lydsy.com/JudgeOnline/problem.php?id=3308

46.http://www.lydsy.com/JudgeOnline/problem.php?id=3996

47.http://www.lydsy.com/JudgeOnline/problem.php?id=3272

48.http://www.lydsy.com/JudgeOnline/problem.php?id=3931

49.http://www.lydsy.com/JudgeOnline/problem.php?id=1797

50.http://www.lydsy.com/JudgeOnline/problem.php?id=3894

51.http://www.lydsy.com/JudgeOnline/problem.php?id=1283

52.http://www.lydsy.com/JudgeOnline/problem.php?id=3144

53.http://www.lydsy.com/JudgeOnline/problem.php?id=2756

54.http://www.lydsy.com/JudgeOnline/problem.php?id=2400

55.http://www.lydsy.com/JudgeOnline/problem.php?id=1149

56.http://www.lydsy.com/JudgeOnline/problem.php?id=2718

57.http://www.lydsy.com/JudgeOnline/problem.php?id=2895

58.http://www.lydsy.com/JudgeOnline/problem.php?id=1565

59.http://www.lydsy.com/JudgeOnline/problem.php?id=2007

60.http://www.lydsy.com/JudgeOnline/problem.php?id=2893

61.http://www.lydsy.com/JudgeOnline/problem.php?id=2929

62.http://www.lydsy.com/JudgeOnline/problem.php?id=1520

63.http://www.lydsy.com/JudgeOnline/problem.php?id=2324

64.http://www.lydsy.com/JudgeOnline/problem.php?id=3396

65.http://www.lydsy.com/JudgeOnline/problem.php?id=3504

66.http://www.lydsy.com/JudgeOnline/problem.php?id=1532

67.http://www.lydsy.com/JudgeOnline/problem.php?id=1930

68.http://www.lydsy.com/JudgeOnline/problem.php?id=2661

69.http://www.lydsy.com/JudgeOnline/problem.php?id=1061

70.http://www.lydsy.com/JudgeOnline/problem.php?id=1711

71.http://www.lydsy.com/JudgeOnline/problem.php?id=2879

72.http://www.lydsy.com/JudgeOnline/problem.php?id=3275

73.http://www.lydsy.com/JudgeOnline/problem.php?id=2768

74.http://www.lydsy.com/JudgeOnline/problem.php?id=2245

75.http://www.lydsy.com/JudgeOnline/problem.php?id=1391

76.http://www.lydsy.com/JudgeOnline/problem.php?id=2127

77.http://www.lydsy.com/JudgeOnline/problem.php?id=2132

78.http://www.lydsy.com/JudgeOnline/problem.php?id=3171

79.http://www.lydsy.com/JudgeOnline/problem.php?id=2424

80.http://www.lydsy.com/JudgeOnline/problem.php?id=1221

81.http://www.lydsy.com/JudgeOnline/problem.php?id=1305

82.http://www.lydsy.com/JudgeOnline/problem.php?id=1066

83.http://poj.org/problem?id=1637

84.http://hihocoder.com/problemset/problem/1393

85.http://hihocoder.com/problemset/problem/1394

86.http://hihocoder.com/problemset/problem/1398

87.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1325

88.http://acm.split.hdu.edu.cn/showproblem.php?pid=3879

89.http://acm.split.hdu.edu.cn/showproblem.php?pid=3871

90.https://nanti.jisuanke.com/t/15549

91.http://acm.split.hdu.edu.cn/showproblem.php?pid=5772

92.http://acm.split.hdu.edu.cn/showproblem.php?pid=4888

93.http://acm.split.hdu.edu.cn/showproblem.php?pid=6214

94.http://acm.split.hdu.edu.cn/showproblem.php?pid=1569

95.http://www.lydsy.com/JudgeOnline/problem.php?id=4873

96.http://www.lydsy.com/JudgeOnline/problem.php?id=3232

97.http://www.lydsy.com/JudgeOnline/problem.php?id=5037

98.http://www.lydsy.com/JudgeOnline/problem.php?id=3438

99.http://www.lydsy.com/JudgeOnline/problem.php?id=3041

100.http://poj.org/problem?id=2125

101.http://acm.split.hdu.edu.cn/showproblem.php?pid=1530

102.http://acm.split.hdu.edu.cn/showproblem.php?pid=3585

103.http://acm.split.hdu.edu.cn/showproblem.php?pid=5277

104.http://acm.split.hdu.edu.cn/showproblem.php?pid=5458

105.http://acm.split.hdu.edu.cn/showproblem.php?pid=5556

106.http://poj.org/problem?id=2400

107.http://poj.org/problem?id=3281

108.http://poj.org/problem?id=3469

109.http://poj.org/problem?id=2195

110.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2071

111.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2760

112.https://cn.vjudge.net/problem/SGU-242

113.http://poj.org/problem?id=1149

114.http://poj.org/problem?id=3498

115.http://poj.org/problem?id=2391

116.http://poj.org/problem?id=2112

117.http://poj.org/problem?id=2455

118.http://poj.org/problem?id=1698

119.http://poj.org/problem?id=1459

120.http://poj.org/problem?id=1087

121.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3976

122.https://cn.vjudge.net/problem/SGU-438

123.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2071

124.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2532

125.http://poj.org/problem?id=1815

126.http://poj.org/problem?id=3204

127.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2587

128.http://poj.org/problem?id=1966

129.http://www.spoj.com/problems/OPTM/

130.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2676

131.http://poj.org/problem?id=3155

132.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3241

133.http://acm.hdu.edu.cn/showproblem.php?pid=3157

134.https://cn.vjudge.net/problem/SGU-176

135.http://poj.org/problem?id=2175

136.http://poj.org/problem?id=3422

137.http://poj.org/problem?id=2516

138.http://poj.org/problem?id=2699

139.http://poj.org/problem?id=3084

140.http://poj.org/problem?id=3189

141.http://poj.org/problem?id=3308

142.http://codeforces.com/problemset/problem/884/F

143.http://codeforces.com/problemset/problem/877/F

144.http://codeforces.com/problemset/problem/818/G

145.http://codeforces.com/gym/101564   （D题）

146.http://codeforces.com/gym/101981/attachments I题






【网络流复习·强化】


1.http://codeforces.com/problemset/problem/808/F

2.http://codeforces.com/problemset/problem/818/G

3.http://codeforces.com/problemset/problem/813/D

4.http://codeforces.com/problemset/problem/802/O

5.http://codeforces.com/problemset/problem/793/G

6.http://codeforces.com/problemset/problem/786/E

7.http://codeforces.com/problemset/problem/736/E

8.http://codeforces.com/problemset/problem/739/E

9.http://codeforces.com/problemset/problem/730/I

10.http://codeforces.com/problemset/problem/727/D

11.http://codeforces.com/problemset/problem/724/E

12.http://codeforces.com/problemset/problem/723/E

13.http://codeforces.com/problemset/problem/717/G

14.http://codeforces.com/problemset/problem/708/D

15.http://codeforces.com/problemset/problem/704/D

16.http://codeforces.com/problemset/problem/720/B

17.http://codeforces.com/problemset/problem/653/D

18.http://codeforces.com/problemset/problem/628/F

19.http://codeforces.com/problemset/problem/611/H

20.http://codeforces.com/problemset/problem/589/F

21.http://codeforces.com/problemset/problem/546/E

22.http://codeforces.com/problemset/problem/498/C

23.http://codeforces.com/problemset/problem/491/C

24.http://codeforces.com/problemset/problem/78/E

25.http://uoj.ac/problem/77

26.http://uoj.ac/problem/132

27.http://uoj.ac/problem/85

28.http://codeforces.com/problemset/problem/863/F








【8】2-sat问题

学习：

http://blog.csdn.net/jarjingx/article/details/8521690




1.http://www.lydsy.com/JudgeOnline/problem.php?id=1997

2.http://hzwer.com/5711.html

3.http://www.lydsy.com/JudgeOnline/problem.php?id=1823

4.http://poj.org/problem?id=3683

5.http://poj.org/problem?id=3207

6.http://www.lydsy.com/JudgeOnline/problem.php?id=4945

7.http://blog.csdn.net/braketbn/article/details/51865230

8.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=010435 B

首先建到达关系的图，缩完点后发现一个物品会被取到至少要访问到横线或竖线中一个，就是在新的DAG途中的两个点，题目转化为固定起点，判断在DAG中是否存在路径可以经过所有限制中至少一个，用2-sat建图求解。然后这个对普通应该图也是可行的，只是复杂度是O(n^2)的。

总结：

http://www.cnblogs.com/-ZZB-/p/6635483.html

【综合应用】

8.http://codeforces.com/problemset/problem/193/A

9.http://codeforces.com/problemset/problem/780/D

10.http://codeforces.com/problemset/problem/776/D

11.http://codeforces.com/problemset/problem/587/D

12.http://codeforces.com/problemset/problem/568/C

13.http://codeforces.com/problemset/problem/538/H

14.http://codeforces.com/problemset/problem/538/H

15.http://codeforces.com/problemset/problem/228/E

16.http://codeforces.com/problemset/problem/27/D

17.https://arc069.contest.atcoder.jp/tasks/arc069_d


【9】图论基础经典题·拓扑排序

1.http://codeforces.com/problemset/problem/915/D

2.http://codeforces.com/problemset/problem/909/E

【10】图的搜索树的构造与应用

http://codeforces.com/problemset/problem/990/F

【11】线段树优化建图

【12】弦图及其性质

【13】瓶颈路

【14】图的可图性质

Havel–Hakimi algorithm：

https://en.wikipedia.org/wiki/Havel%E2%80%93Hakimi_algorithm

Erdős–Gallai theorem：

https://en.wikipedia.org/wiki/Erd%C5%91s%E2%80%93Gallai_theorem

1.http://codeforces.com/problemset/problem/1091/E

注：n+1个点的无向简单图，给定其中n个点的度序列，问最后一个点的度数取值集合

结论：握手定理，且答案构成或奇或偶一个连续区间

由Erdős–Gallai theorem知，需要符合n+1个不等式，最后一个显然成立，也就是要满足n个条件；对每个条件，单独计算答案的可能区间，区间加1；全部做完，看哪些值的标记达到n；使用差分思想，时间复杂度O(n)





# 4.字符串

【1】KMP与扩展KMP（重点）

指定题目：

1.http://acm.hdu.edu.cn/showproblem.php?pid=4333

2.http://codeforces.com/contest/535/problem/D

3.http://codeforces.com/contest/631/problem/D

4.http://www.lydsy.com/JudgeOnline/problem.php?id=3620

5.http://poj.org/problem?id=2406

6.http://poj.org/problem?id=3461

7.http://poj.org/problem?id=2752

8.http://poj.org/problem?id=1961

9.http://poj.org/problem?id=2185

10.http://poj.org/problem?id=3080

11.http://acm.hdu.edu.cn/showproblem.php?pid=4763

12.http://acm.hdu.edu.cn/showproblem.php?pid=3613

13.http://acm.hdu.edu.cn/showproblem.php?pid=4300

14.http://acm.hdu.edu.cn/showproblem.php?pid=4763

15.http://acm.hdu.edu.cn/showproblem.php?pid=5782

16.http://codeforces.com/problemset/problem/808/G




【2】RK算法与字符串hash（线性预处理区间hash）（重点）

1.http://codeforces.com/contest/608/problem/E

2.http://acm.hdu.edu.cn/showproblem.php?pid=3973

3.http://acm.hdu.edu.cn/showproblem.php?pid=6046

4.http://acm.hdu.edu.cn/showproblem.php?pid=4821

5.http://acm.hdu.edu.cn/showproblem.php?pid=5414

6.http://acm.hdu.edu.cn/showproblem.php?pid=4622（字符串hash+线段树）

7.http://acdream.info/problem?pid=1019

8.http://codeforces.com/contest/580/problem/E

9.http://codeforces.com/problemset/problem/835/D

10.http://codeforces.com/problemset/problem/7/D

11.http://codeforces.com/problemset/problem/25/E

12.http://codeforces.com/problemset/problem/119/D

13.http://codeforces.com/problemset/problem/316/G1

14.http://codeforces.com/problemset/problem/958/A2

注：二维hash，每个方向一个base，公共模数，注意高低位统一

15.http://codeforces.com/problemset/problem/580/E

注：线段树区间替换，区间查询hash值

16.http://codeforces.com/group/aUVPeyEnI2/contest/243686 C题

注：对每个本质不同子串，抠出所有出现下标集合，利用字符串hash判等





【3】字典Trie树/Manacher（重点）

01字典树专题：http://blog.csdn.net/miracle_ma/article/details/51484054

1.http://acm.hdu.edu.cn/showproblem.php?pid=1251

2.http://codeforces.com/contest/159/problem/D

3.http://acm.hdu.edu.cn/showproblem.php?pid=1251

4.http://www.lydsy.com/JudgeOnline/problem.php?id=4260

5.http://www.lydsy.com/JudgeOnline/problem.php?id=4567

6.http://www.lydsy.com/JudgeOnline/problem.php?id=2741

7.http://codeforces.com/problemset/problem/557/E

注：经典的01字典树上求k大值问题，形式类似于：问给定01串中所有子串字典序k大的子串，O(n^2)







【4】AC自动机/Trie图（重点）

1.http://codeforces.com/contest/697/problem/F

2.http://codeforces.com/contest/710/problem/F

3.http://codeforces.com/contest/86/problem/C

4.http://codeforces.com/contest/7/problem/D

5.http://poj.org/problem?id=2778

6.http://www.lydsy.com/JudgeOnline/problem.php?id=1030

7.http://acm.hdu.edu.cn/showproblem.php?pid=2222

8.http://poj.org/problem?id=2000

9.http://www.lydsy.com/JudgeOnline/problem.php?id=2434（用ac自动机做）

10.http://www.lydsy.com/JudgeOnline/problem.php?id=1195

11.http://www.lydsy.com/JudgeOnline/problem.php?id=1009

12.http://www.lydsy.com/JudgeOnline/problem.php?id=1212

13.http://www.lydsy.com/JudgeOnline/problem.php?id=3530

14.http://www.lydsy.com/JudgeOnline/problem.php?id=1030

15.http://www.lydsy.com/JudgeOnline/problem.php?id=1039

16.http://www.lydsy.com/JudgeOnline/problem.php?id=2553

17.http://www.lydsy.com/JudgeOnline/problem.php?id=3172

18.http://www.lydsy.com/JudgeOnline/problem.php?id=1444

19.http://www.lydsy.com/JudgeOnline/problem.php?id=1559

20.http://acm.hdu.edu.cn/showproblem.php?pid=5880

21.http://acm.hdu.edu.cn/showproblem.php?pid=2896

22.http://acm.hdu.edu.cn/showproblem.php?pid=3695

23.http://acm.hdu.edu.cn/showproblem.php?pid=2296

24.http://acm.hdu.edu.cn/showproblem.php?pid=6138

25.http://acm.hdu.edu.cn/showproblem.php?pid=4117

26.http://acm.hdu.edu.cn/showproblem.php?pid=4518

27.http://acm.hdu.edu.cn/showproblem.php?pid=5955

28.http://acm.hdu.edu.cn/showproblem.php?pid=4534

29.http://acm.hdu.edu.cn/showproblem.php?pid=6096

30.http://acm.hdu.edu.cn/showproblem.php?pid=6086

31.http://acm.hdu.edu.cn/showproblem.php?pid=5384

32.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2619

33.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3494

34.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3545

35.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3190

36.https://uva.onlinejudge.org/index.php?option=com_onlinejudge&Itemid=8&category=26&page=show_problem&problem=2463

37.https://uva.onlinejudge.org/index.php?option=com_onlinejudge&Itemid=8&category=22&page=show_problem&problem=1960

38.http://acm.hdu.edu.cn/showproblem.php?pid=2243

39.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=1540

40.http://acm.hdu.edu.cn/showproblem.php?pid=2825

41.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3013

42.http://poj.org/problem?id=3691

43.http://acm.hdu.edu.cn/showproblem.php?pid=3341

44.http://codeforces.com/problemset/problem/1110/H

注：trie图+数位dp+正则表达式通配符状态表示

45.http://codeforces.com/problemset/problem/710/F

注：经典的强制在线ac自动机，参见二进制分组算法







【5】后缀数组(重点)

1.http://poj.org/problem?id=2774

2.http://acm.hdu.edu.cn/showproblem.php?pid=4622（同样的题目）

3.http://www.lydsy.com/JudgeOnline/problem.php?id=4310

4.http://www.lydsy.com/JudgeOnline/problem.php?id=4946

5.http://www.cnblogs.com/SiriusRen/p/6654401.html

6.http://www.lydsy.com/JudgeOnline/problem.php?id=3172

7.http://hzwer.com/3605.html

8.http://www.lydsy.com/JudgeOnline/problem.php?id=4552

9.http://hzwer.com/7454.html

10.http://codeforces.com/contest/204/problem/E

11.http://www.lydsy.com/JudgeOnline/problem.php?id=2119

12.http://www.lydsy.com/JudgeOnline/problem.php?id=4566（用后缀数组）

13.http://www.lydsy.com/JudgeOnline/problem.php?id=4516

14.http://www.lydsy.com/JudgeOnline/problem.php?id=3998

15.http://www.lydsy.com/JudgeOnline/problem.php?id=4199（百度搜题目，只可以评测）

16.http://www.lydsy.com/JudgeOnline/problem.php?id=3238

`2` `20190605` `bzoj3238` `SAM` `后缀树`

17.http://www.lydsy.com/JudgeOnline/problem.php?id=1031

18.http://hzwer.com/4248.html

19.http://www.lydsy.com/JudgeOnline/problem.php?id=3879

`2` `20190605` `bzoj3879` `虚树` `SAM` `后缀树`

前置技能是 `bzoj3238`

20.http://www.lydsy.com/JudgeOnline/problem.php?id=2754

21.http://www.lydsy.com/JudgeOnline/problem.php?id=2534

22.http://www.lydsy.com/JudgeOnline/problem.php?id=3676

23.http://codeforces.com/contest/700/problem/E

24.http://codeforces.com/contest/427/problem/D

25.http://codeforces.com/contest/452/problem/E

26.http://codeforces.com/contest/432/problem/D

27.http://codeforces.com/contest/123/problem/D

28.http://codeforces.com/contest/128/problem/B

29.http://codeforces.com/problemset/problem/825/F

30.http://codeforces.com/problemset/problem/822/E

31.http://codeforces.com/problemset/problem/727/E

32.http://codeforces.com/problemset/problem/710/F

33.http://poj.org/problem?id=1743

34.http://poj.org/problem?id=3261

35.http://poj.org/problem?id=2406

36.http://poj.org/problem?id=3693

37.http://poj.org/problem?id=3294

38.http://poj.org/problem?id=3415

39.http://www.spoj.com/problems/DISUBSTR/

40.http://acm.timus.ru/problem.aspx?space=1&num=1297

41.http://acm.timus.ru/problem.aspx?space=1&num=1517

42.http://www.spoj.com/problems/REPEATS/

43.http://www.spoj.com/problems/PHRASES/

44.http://poj.org/problem?id=1226

45.http://hihocoder.com/problemset/problem/1419

46.http://hihocoder.com/problemset/problem/1403

47.http://hihocoder.com/problemset/problem/1407

48.http://hihocoder.com/problemset/problem/1415

49.https://nanti.jisuanke.com/t/31717





【6】后缀树



【7】后缀自动机

1.http://hihocoder.com/problemset/problem/1441

2.http://hihocoder.com/problemset/problem/1445

3.http://hihocoder.com/problemset/problem/1449

4.http://hihocoder.com/problemset/problem/1457

5.http://hihocoder.com/problemset/problem/1465

6.http://hihocoder.com/problemset/problem/1466

7.http://www.lydsy.com/JudgeOnline/problem.php?id=3676

8.http://www.lydsy.com/JudgeOnline/problem.php?id=3238

9.http://www.lydsy.com/JudgeOnline/problem.php?id=3926

10.http://www.lydsy.com/JudgeOnline/problem.php?id=1921

11.http://www.lydsy.com/JudgeOnline/problem.php?id=3473

12.http://www.lydsy.com/JudgeOnline/problem.php?id=1396

13.http://www.lydsy.com/JudgeOnline/problem.php?id=3145



【8】回文树/回文自动机/Eertree

一篇文章：http://codeforces.com/blog/entry/13959

加速dp转移(有专门模板和论文、题目)：

https://blog.bill.moe/dp-with-palindrome-notes/

http://codeforces.com/blog/entry/19193



1.http://acm.split.hdu.edu.cn/showproblem.php?pid=4426

2.https://vjudge.net/contest/189299#problem/G

3.http://acm.timus.ru/problem.aspx?space=1&num=1960

4.http://www.tsinsen.com/A1280

5.http://www.tsinsen.com/A1255

6.http://www.tsinsen.com/A1393

7.http://acm.split.hdu.edu.cn/showproblem.php?pid=5394

8.http://www.lydsy.com/JudgeOnline/problem.php?id=3676

9.https://www.codechef.com/problems/PALPROB

10.http://www.lydsy.com/JudgeOnline/problem.php?id=4567

11.http://www.lydsy.com/JudgeOnline/problem.php?id=2160

12.http://www.lydsy.com/JudgeOnline/problem.php?id=2084

13.http://www.lydsy.com/JudgeOnline/problem.php?id=2342

14.http://www.lydsy.com/JudgeOnline/problem.php?id=2565

15.http://www.lydsy.com/JudgeOnline/problem.php?id=3160

16.http://www.lydsy.com/JudgeOnline/problem.php?id=3672

17.http://www.lydsy.com/JudgeOnline/problem.php?id=4044

18.http://acm.timus.ru/problem.aspx?space=1&num=2057

19.http://acm.timus.ru/problem.aspx?space=1&num=2058

20.http://acm.timus.ru/problem.aspx?space=1&num=2059

21.http://acm.timus.ru/problem.aspx?space=1&num=2060

22.http://acm.timus.ru/problem.aspx?space=1&num=2061

23.http://acm.timus.ru/problem.aspx?space=1&num=2044

24.http://www.spoj.com/problems/IITKWPCE/

25.http://acm.timus.ru/problem.aspx?space=1&num=1635

26.http://codeforces.com/problemset/problem/906/E

27.https://nanti.jisuanke.com/t/30998


【9】后缀仙人掌


【10】后缀平衡树


【11】广义后缀树/广义后缀自动机

1.http://www.lydsy.com/JudgeOnline/problem.php?id=3926

2.http://www.lydsy.com/JudgeOnline/problem.php?id=3277

3.http://www.lydsy.com/JudgeOnline/problem.php?id=3473

4.http://www.lydsy.com/JudgeOnline/problem.php?id=4545

5.http://www.lydsy.com/JudgeOnline/problem.php?id=2780

6.http://www.lydsy.com/JudgeOnline/problem.php?id=2806

7.http://www.lydsy.com/JudgeOnline/problem.php?id=4199



【12】可持久化回文自动机/后缀自动机

【13】Border Tree

【14】序列自动机

定义：给定一个序列$a$，下标$[1,n]$，它的序列自动机是一个有向图$DAG$，构造如下：

新建$0$号点$S$和$n+1$号点$T$，对每个下标$i$建一个点$i$，$\forall i \in [0,n]$，$i$向右连出$c$条有向边($c$为字符集大小)，连向字符集中的每个字符在下标$i$右侧第一次出现的下标，对于没有出现的字符，连向$T$

**目前已知的性质：**

1)可以识别序列$a$的所有子序列，注意除$S,T$之外每个点均为可接受点

2)可以求序列$a$本质不同的子序列个数，具体来说，$\forall i \in [1,n]$，可以计算$f[i]$表示以下标$i$结尾且下标$i$必取的本质不同子序列个数，$f[T]$即为整个序列$a$的本质不同子序列个数，对$f$求前缀和即得前缀中的本质不同子序列个数，$f$数组本身可以在$DAG$上做$dp$计算，注意此用法不要保留多重边

证明：序列自动机(无重边)上$S$到$T$的通路与序列$a$的所有本质不同子序列(包括空子序列)一一对应

事实上，任取两条不同的通路，若它们代表的字符连接构成的字符串相同，则取它们第一个不同的下标$p,q$，和最后一个相同的下标$t$，则说明$a[p]=a[q]$且$p \ne q$，这与$t$对于字符$a[p]$只有一条出边矛盾

3)序列自动机的最短路长度等于序列$a$的密度$+1$，参见组合$dp$中的$codeforces \space 1158F$词条

证明：沿用组合$dp$那道题目的说法，假设序列$a$，含有$k$个块，字符集大小为$c$

事实上，$S$到$T$的任一条通路，都至少要经过每个块至少一次，最后还需要一次跳出，故$len \ge k+1$

另一方面，显然可以构造出以下路径确实$len=k+1$，从而可以使得不等号取到等号：

从$S$开始，依次经过每个块的末端点，最后跳出到$T$



【15】最小表示法







# 5.dp深入

##【1】几类经典dp：数位dp

指定题目：

1.http://codeforces.com/contest/55/problem/D

2.http://codeforces.com/contest/628/problem/D

3.http://codeforces.com/contest/747/problem/F

4.http://codeforces.com/contest/259/problem/D

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3598

6.http://www.lydsy.com/JudgeOnline/problem.php?id=1833

7.http://www.lydsy.com/JudgeOnline/problem.php?id=1026

8.http://www.lydsy.com/JudgeOnline/problem.php?id=3131

9.http://www.lydsy.com/JudgeOnline/problem.php?id=4521

10.http://acm.hdu.edu.cn/showproblem.php?pid=5435

11.http://acm.hdu.edu.cn/showproblem.php?pid=4722

12.http://acm.hdu.edu.cn/showproblem.php?pid=3555

13.http://acm.hdu.edu.cn/showproblem.php?pid=3652

14.http://acm.hdu.edu.cn/showproblem.php?pid=4734

15.http://acm.hdu.edu.cn/showproblem.php?pid=5787

16.http://acm.hdu.edu.cn/showproblem.php?pid=5898

17.http://acm.hdu.edu.cn/showproblem.php?pid=3886

18.http://acm.hdu.edu.cn/showproblem.php?pid=5808

19.http://acm.hdu.edu.cn/showproblem.php?pid=3943

20.http://acm.hdu.edu.cn/showproblem.php?pid=6156

21.http://acm.hdu.edu.cn/showproblem.php?pid=4352


自由题目：自己做专题

##【2】dp优化：四边形不等式

指定题目：

1.http://www.lydsy.com/JudgeOnline/problem.php?id=1010

2.http://acm.hdu.edu.cn/showproblem.php?pid=3480

3.http://acm.hdu.edu.cn/showproblem.php?pid=2829

4.http://acm.hdu.edu.cn/showproblem.php?pid=3506

5.http://acm.hdu.edu.cn/showproblem.php?pid=3516

6.http://codeforces.com/problemset/problem/321/E

7.http://poj.org/problem?id=1160

8.http://www.lydsy.com/JudgeOnline/problem.php?id=1563

9.http://www.lydsy.com/JudgeOnline/problem.php?id=2216

10.http://www.lydsy.com/JudgeOnline/problem.php?id=2739

11.http://www.lydsy.com/JudgeOnline/problem.php?id=3229

12.http://www.lydsy.com/JudgeOnline/problem.php?id=3675

13.http://www.lydsy.com/JudgeOnline/problem.php?id=4367

14.http://www.lydsy.com/JudgeOnline/problem.php?id=4426

## 【3】dp优化：单调队列与单调栈


【文章】http://blog.csdn.net/LZJ209/article/details/76150259


1.http://acm.hdu.edu.cn/showproblem.php?pid=3401

2.http://acm.hdu.edu.cn/showproblem.php?pid=3410

3.http://acm.hdu.edu.cn/showproblem.php?pid=1500

4.http://acm.hdu.edu.cn/showproblem.php?pid=1059

5.http://acm.hdu.edu.cn/showproblem.php?pid=4123

6.http://www.lydsy.com/JudgeOnline/problem.php?id=1855

7.https://www.lydsy.com/JudgeOnline/problem.php?id=3831

8.https://www.lydsy.com/JudgeOnline/problem.php?id=3048

9.http://www.lydsy.com/JudgeOnline/problem.php?id=1499

10.https://www.lydsy.com/JudgeOnline/problem.php?id=2096

11.https://www.lydsy.com/JudgeOnline/problem.php?id=3126

12.https://www.lydsy.com/JudgeOnline/problem.php?id=1127

13.https://nanti.jisuanke.com/t/30991

14.https://www.lydsy.com/JudgeOnline/problem.php?id=1342

15.https://www.lydsy.com/JudgeOnline/problem.php?id=2500

16.http://www.lydsy.com/JudgeOnline/problem.php?id=3316

17.http://www.lydsy.com/JudgeOnline/problem.php?id=1012

18.http://www.lydsy.com/JudgeOnline/problem.php?id=1023

19.https://www.lydsy.com/JudgeOnline/problem.php?id=1233

20.https://www.lydsy.com/JudgeOnline/problem.php?id=1122

21.http://codeforces.com/problemset/problem/939/F

22.http://codeforces.com/problemset/problem/940/E

23.http://codeforces.com/problemset/problem/960/F











## 【4】dp优化：斜率优化

【参考】http://blog.csdn.net/cdqzoiers/article/details/52497160

https://codeforces.com/blog/entry/8219



1.http://www.lydsy.com/JudgeOnline/problem.php?id=4518

2.http://www.lydsy.com/JudgeOnline/problem.php?id=4073

3.http://www.lydsy.com/JudgeOnline/problem.php?id=4578

4.http://www.lydsy.com/JudgeOnline/problem.php?id=2726

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3963

6.http://www.lydsy.com/JudgeOnline/problem.php?id=1010

7.http://www.lydsy.com/JudgeOnline/problem.php?id=1911

8.http://www.lydsy.com/JudgeOnline/problem.php?id=3156

9.http://www.lydsy.com/JudgeOnline/problem.php?id=4517

10.http://www.lydsy.com/JudgeOnline/problem.php?id=1767

11.http://www.lydsy.com/JudgeOnline/problem.php?id=2442

12.http://codeforces.com/problemset/problem/643/C

13.http://codeforces.com/problemset/problem/631/E

14.http://codeforces.com/problemset/problem/673/E

15.http://acm.hdu.edu.cn/showproblem.php?pid=3480

16.http://acm.hdu.edu.cn/showproblem.php?pid=3480

17.http://acm.hdu.edu.cn/showproblem.php?pid=2829

18.http://acm.hdu.edu.cn/showproblem.php?pid=3507

19.http://acm.hdu.edu.cn/showproblem.php?pid=3545

20.http://acm.hdu.edu.cn/showproblem.php?pid=2993

21.http://www.lydsy.com/JudgeOnline/problem.php?id=1492

22.http://www.lydsy.com/JudgeOnline/problem.php?id=3672

23.http://acm.hdu.edu.cn/showproblem.php?pid=3725

24.https://www.lydsy.com/JudgeOnline/problem.php?id=5380



## 【5】dp优化：利用各种数据结构优化转移

1.http://codeforces.com/contest/834/problem/D

2.http://www.lydsy.com/JudgeOnline/problem.php?id=1835

3.https://www.lydsy.com/JudgeOnline/problem.php?id=2933

4.http://www.lydsy.com/JudgeOnline/problem.php?id=4422

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3380

6.http://www.lydsy.com/JudgeOnline/problem.php?id=4417

7.http://codeforces.com/problemset/problem/720/D

8.http://www.lydsy.com/JudgeOnline/problem.php?id=3688

9.http://www.lydsy.com/JudgeOnline/problem.php?id=4361

10.http://www.lydsy.com/JudgeOnline/problem.php?id=3790

11.http://codeforces.com/problemset/problem/573/B

12.http://codeforces.com/contest/474/problem/E

13.http://codeforces.com/contest/675/problem/E

14.http://codeforces.com/contest/777/problem/E

15.http://codeforces.com/contest/573/problem/D

16.http://codeforces.com/contest/115/problem/E

17.http://codeforces.com/contest/629/problem/D

18.http://codeforces.com/contest/487/problem/B

19.http://codeforces.com/problemset/problem/809/D

20.http://codeforces.com/problemset/problem/939/F

21.http://codeforces.com/problemset/problem/958/C3





## 【6】几类经典dp：状态压缩动态规划/状压dp与插头dp

看论文，和一些资料：http://www.cnblogs.com/kuangbin/archive/2012/10/02/2710343.html

1.http://www.lydsy.com/JudgeOnline/problem.php?id=1072

​	问有多少数字排列整除d，对余数装压

2.http://www.lydsy.com/JudgeOnline/problem.php?id=1087

​	问N*N棋盘放k个国王有几种方案，需要先预处理两层之间的转移，不然复杂度不够

X 3.http://www.lydsy.com/JudgeOnline/problem.php?id=119

4.http://www.lydsy.com/JudgeOnline/problem.php?id=1879

​	状压dp计数，状压dp要注意预处理转移，减少复杂度 

5.http://www.lydsy.com/JudgeOnline/problem.php?id=2064

​	两堆数，每次可以合并两个，问最少几次可以两堆一样, 转移分步的思想要注意，可以减少复杂度 

6.http://www.lydsy.com/JudgeOnline/problem.php?id=3717

​	n个物品放入m个包里，最少要几个包，状态为用了哪些物品，考虑状态之间的有序性，逐个插入物品

7.http://www.lydsy.com/JudgeOnline/problem.php?id=3812

​	n点m边强连通子图计数，首先要会n点m边DAG计数，然后把枚举出度为零的点集容斥改为枚举缩点后出度为零的点集容斥

8.http://www.lydsy.com/JudgeOnline/problem.php?id=4057

​	简单的状态表示和转移

9.http://www.lydsy.com/JudgeOnline/problem.php?id=4145

​	状态为已经有哪些物品，分步转移优化

10.http://www.lydsy.com/JudgeOnline/problem.php?id=4455

​	给n个点的图和树，给树不重复标号，树上边要在图中出现。用容斥来保证标号不重复，有重复标号等价于有标号没用到

11.http://www.lydsy.com/JudgeOnline/problem.php?id=4565

​	一个01串可选k个合并为一个，得到对应2^k种权值中一个，求最大价值，区间dp，主要把合并过程看成一棵树，枚举后缀为0或1以及前缀的状态合并 

12.http://www.lydsy.com/JudgeOnline/problem.php?id=4600

13.http://www.lydsy.com/JudgeOnline/problem.php?id=4601

14.http://acm.hdu.edu.cn/showproblem.php?pid=4049

​	层之间的有序性要考虑清楚，最好写成分层的形式

15.http://acm.hdu.edu.cn/showproblem.php?pid=3920

​	每次给固定选一个再枚举一个转移，复杂度低一些

16.http://acm.hdu.edu.cn/showproblem.php?pid=1074

​	简单题

17.http://acm.hdu.edu.cn/showproblem.php?pid=5067

​	TSP问题

18.http://acm.hdu.edu.cn/showproblem.php?pid=4997

​	求边双联通子图个数, 需要容斥计算联通子图，不联通子图，单联通子图个数

19.http://acm.hdu.edu.cn/showproblem.php?pid=4336

20.http://acm.hdu.edu.cn/showproblem.php?pid=1074

21.http://acm.hdu.edu.cn/showproblem.php?pid=5094

​	bfs过程中对每个点开个状态来表示

22.http://acm.hdu.edu.cn/showproblem.php?pid=2820

​	求相邻差值小于等于k(k<=4)的排列数量，一种枚举排列的方法，考虑有序插入数字，那么已有的数字可以表示成一些段，转移主要有合并，连接，新增一段，还要注意考虑边界状态。

23.http://acm.hdu.edu.cn/showproblem.php?pid=3471

24.http://acm.hdu.edu.cn/showproblem.php?pid=1565

25.http://acm.hdu.edu.cn/showproblem.php?pid=3605

26.http://acm.hdu.edu.cn/showproblem.php?pid=5045

27.http://acm.hdu.edu.cn/showproblem.php?pid=3311

28.http://acm.hdu.edu.cn/showproblem.php?pid=5724

29.http://acm.hdu.edu.cn/showproblem.php?pid=4295

30.http://acm.hdu.edu.cn/showproblem.php?pid=3006

31.http://acm.hdu.edu.cn/showproblem.php?pid=5418

32.http://acm.hdu.edu.cn/showproblem.php?pid=4352

33.http://acm.hdu.edu.cn/showproblem.php?pid=4628

34.http://acm.hdu.edu.cn/showproblem.php?pid=1885

35.http://acm.hdu.edu.cn/showproblem.php?pid=4284

36.http://acm.hdu.edu.cn/showproblem.php?pid=3001

37.https://www.lydsy.com/JudgeOnline/problem.php?id=5369

38.http://poj.org/problem?id=2411

39.http://poj.org/problem?id=1739

40.http://acm.hdu.edu.cn/showproblem.php?pid=1693

41.http://acm.hdu.edu.cn/showproblem.php?pid=4949

42.http://acm.hdu.edu.cn/showproblem.php?pid=4804

43.http://acm.hdu.edu.cn/showproblem.php?pid=5731

44.http://acm.hdu.edu.cn/showproblem.php?pid=4064

45.http://acm.hdu.edu.cn/showproblem.php?pid=4285

46.http://acm.fzu.edu.cn/problem.php?pid=1977

47.http://acm.timus.ru/problem.aspx?space=1&num=1519

48.http://acm.hdu.edu.cn/showproblem.php?pid=3377

49.http://poj.org/problem?id=3133

50.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3446

51.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3256

52.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3213

53.http://codeforces.com/problemset/problem/906/C

54.http://codeforces.com/problemset/problem/1097/H

[注]经典的三段论区间合并式状压dp + bitset状态表示 + 倍增/递归处理计数

55.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=010433 C

​	关键在于用floyd处理团之间距离，注意每个点的初始花费最后再加，然后就转化成有2^k类点，两类点的距离是包含的团之间的距离的最小值，这样枚举复杂度还不够，改为从小到大枚举最短路，再枚举第一个点，和它距离是这条最短路的点数量用子集和来维护，然后标记第一个枚的点和这些点已经算过了，下次不再算，因为已经有较短的路了。



## 【7】几类经典dp：背包问题

1.http://codeforces.com/problemset/problem/868/E

2.http://codeforces.com/problemset/problem/920/D

3.http://codeforces.com/problemset/problem/946/D



## 【8】几类经典dp：树形dp

1.http://codeforces.com/contest/766/problem/E

2.http://codeforces.com/problemset/problem/868/E

3.http://codeforces.com/problemset/problem/935/E

4.http://codeforces.com/problemset/problem/960/E

5.http://codeforces.com/problemset/problem/963/B

6.http://codeforces.com/problemset/problem/1065/F

7.http://codeforces.com/problemset/problem/1092/F

注：树上换根，计算全局贡献

8.http://codeforces.com/problemset/problem/1097/G

注：经典且稍复杂的树上合并式背包，需容斥

9.http://codeforces.com/problemset/problem/1153/D

注：树形dp，这种max/min绕来绕去的题目往往一个点的状态和某个离散化后的集合排名有关，结合简单的贪心思想，此排名可转移

10.http://codeforces.com/problemset/problem/1059/E

注 ：这题用贪心比较容易做，每次从叶子把向上最长能覆盖的都盖了，并查集维护被覆盖的点就行了，看了一下题解dp的做法，主要是一个点向下的链可以用从它开始欧拉序的前缀表示，然后比较麻烦，还需要线段树维护限制和答案，每次暴力删除已经不符合的点，因为这次不符合之后也不会再符合

11.http://codeforces.com/problemset/problem/429/C

注 ：给你树上每个点的size，问树是否存在，正解应该是把叶子和非叶子分开状压，一棵树其实应该有多种子树选择方案，我直接贪心加背包选了一种，因为n比较小，可能反例不太有，这样做就可以过

12.http://codeforces.com/problemset/problem/629/E

注 ：问树上两点加一条边成环平均长度，就是树上换根计数

13.http://codeforces.com/problemset/problem/86/C

注 ：问能被一些字符串覆盖的母串有多少种，发现ac自动机一直理解错了，到了一个点要把它fail链上的点都算上贡献

14.http://codeforces.com/problemset/problem/1146/F

注 ：感觉不错的树dp题，问你有多少种叶子划分使其相同集合叶子联通且没有交，要记录三个量，i的子树答案，i是已经被用的数量，i是被虚占用的数量，然后转移要推清楚，我一开始转移搞错了，花了很多时间。

15.http://codeforces.com/problemset/problem/708/C

注 ：问每个点在能换一条边的情况下能否是重心，用树上换根技巧维护每一个点为根时子树中最大的小于n/2的子树size。

16.http://codeforces.com/problemset/problem/490/F

注 ：问你树上所有路径中的最长上升子序列多长，维护向上向下两条链实现

17.http://codeforces.com/problemset/problem/965/E

注 ：建完字典树后就变成树上有一些1，每个1可以往上移，但是每个位子至多一个1，要深度和最小，每次选最深的一个1，找到它向上第一个不为1的位置放过去，可以用并查集实现

18.http://codeforces.com/problemset/problem/804/D

注 ：询问森林中两棵树连一条边期望直径，主要是复杂度上是有分块思想，一次询问的复杂度是较小树的size，那么大于sqrt(n)的点对最多只用n个，所以复杂度是O(nsqrt(n)log(n))

19.http://codeforces.com/problemset/problem/1109/D

注 ：边权范围1-m，问有多少棵无根树a到b的距离是m，有一个prufer序列的结论，详细学了一下prufer序列，记在了它相关的结论中

20.http://codeforces.com/problemset/problem/1032/F

注 ：问一棵树有多少种方法删一个点集使剩下的图最大匹配使唯一的，定义三种状态，i和儿子没边且没匹配，i和儿子有边且没匹配，i和儿子有边且匹配了，然后推一下转移式，然后发现一般转移如果是选儿子的子集，可以用乘法分配律合起来乘

21.http://codeforces.com/problemset/problem/1132/G

注 ：给一个数组，每一位往后面第一个比他大的连边，问所有长度为k区间中最长链是多少，在dfs序上用线段树处理一下就行

22.http://codeforces.com/problemset/problem/123/E

注 ：推出指定根后每个点期望怎么算后套上树上换根即可

性质：在无根树中从一个给定起点S到某个非S节点T的dfs期望步数(包括回溯)为n-size(T)，size为子树大小，看成以S为根的有根树

本质：典型的条件随机变量的数学期望，也就是全期望公式相关，详情参见数学词条

23.http://codeforces.com/problemset/problem/643/E

注 ：发现只有对一个点深度不超过一定值的点才对答案有影响，所以加点更新和算期望可以只算一部分，复杂度就对了。

24.http://acm.hdu.edu.cn/showproblem.php?pid=6060

注 ： 发现根往下每一个子树都是独立的，所以一条边的最大贡献次数是下面size大小和集合数量k取min，这样dfs一遍即可

25.http://codeforces.com/gym/102220/problem/A

注：贪心+二分图Hall定理+暴力维护树dp

$二分图网络流模型左边点满流充要条件:Hall定理$

任取左侧点子集$X$，与之相连的右侧点子集$Y$，则$X$集合所对容量之和$\le$$Y$集合所对容量之和











## 【9】几类经典dp：概率dp

参考：动态规划与计数问题(北京⼤学,洪华敦)  wannafly_2019_winter_div1_计数

1.http://acm.hdu.edu.cn/showproblem.php?pid=4809

注：偏树形dp，和概率关系比较小，树上每个点可分给三个人，每个人消耗他有的奇数联通块数减偶数联通块数的代价，记录i的联通块奇偶性和已有的差值，与儿子转移一下

2.http://codeforces.com/gym/101655  (C题)

注：暴力记忆化转移 

3.https://www.lydsy.com/JudgeOnline/problem.php?id=5340

注：概率的形式可以用多项式表示，以及多项式除两项多项式可以O(n)做到

4.https://www.lydsy.com/JudgeOnline/problem.php?id=2688

注：树上删边的sg函数结论，然后以sg值为状态转移概率，用到二叉树计数

5.https://www.lydsy.com/JudgeOnline/problem.php?id=3450

注：维护连续1平方的期望，知道了期望可以通过维护差值来转移

6.https://www.lydsy.com/JudgeOnline/problem.php?id=4844

注：列出dp方程，优化一下计数方式即可

7.https://www.lydsy.com/JudgeOnline/problem.php?id=4318

注：维护连续1立方的期望，和之前差不多，多维护一项平方的期望

8.https://www.lydsy.com/JudgeOnline/problem.php?id=1246

注：收集n个物品，每次随机买，每买一次价格贵1，问期望多少钱买齐，状态要建立成有i个物品且还没买过东西，这样可以和前面无关，然后化简转移方程

9.https://www.lydsy.com/JudgeOnline/problem.php?id=4820

10.https://www.lydsy.com/JudgeOnline/problem.php?id=5004

注：概率空间有限，其实就是组合计数，dp转移一下，但是题面写有精度判断，但bzoj是直接比较，被坑了不少时间

11.https://www.lydsy.com/JudgeOnline/problem.php?id=3029

注：简单的概率dp，设计dp状态转移一下，一些小技巧，增加偏移量和滚动数组

12.https://www.lydsy.com/JudgeOnline/problem.php?id=2554

注：有一堆有颜色的小球，每次选两个出来，把后面变前面颜色，问期望多少次变一样，先转化成只考虑两种颜色，然后要求条件概率下的期望，其相邻两项转移系数是不同的，以及一个套路，求与左右相邻两项有关的递推式的方法

13.https://www.lydsy.com/JudgeOnline/problem.php?id=3270

或者：http://codeforces.com/problemset/problem/113/D

注：状态图上随机游走，有一些终结态，求停在每个状态的概率，算是通用套路，设经过期望次数，去建立方程，高斯消元，注意二元pair表示状态(重编号)

14.https://www.lydsy.com/JudgeOnline/problem.php?id=2201

注：一个环上每个点随机颜色，问连续颜色长度乘积的期望，枚举第一个长度断环，dp求一下第二个和最后一个颜色和第一个不同的期望

15.https://www.lydsy.com/JudgeOnline/problem.php?id=4008

注：只考虑第一张卡牌，发现期望只和它发布发动有关，和在哪一轮发动无关，所以以此建立状态记忆化转移

16.https://www.lydsy.com/JudgeOnline/problem.php?id=3566

注：树上概率dp加上换根技巧，以及换根的时候要注意运算是否可逆

17.https://www.lydsy.com/JudgeOnline/problem.php?id=2337

注：异或拆位后建图建立方程组高斯消元

18.https://www.lydsy.com/JudgeOnline/problem.php?id=3143

注：计算随机游走的过程中每条边经过的期望次数

19.https://www.lydsy.com/JudgeOnline/problem.php?id=3191

注：简单题，表示一下状态转移，就是环上的下标转移要计算清楚

20.https://www.lydsy.com/JudgeOnline/problem.php?id=5292

注：求出转移方程，发现第i项之和i+1和与它小的项有关系，这样接近与上三角，可以用高斯消元在O(n^2)解决

21.https://www.lydsy.com/JudgeOnline/problem.php?id=5461

或者：https://loj.ac/problem/2537

注：线段树合并(带区间修改标记)+概率dp

树上概率dp经典题，叶子节点带点权，非叶子节点带概率，表示在两个儿子之间选择大的概率，求根的概率分布列；带区间修改的线段树合并，并没有特别之处，注意查询和合并函数中向下递归之前，先push_down

22.https://www.lydsy.com/JudgeOnline/problem.php?id=4720

注：基础传统题，注意多重边，floyed+概率dp

23.https://www.lydsy.com/JudgeOnline/problem.php?id=4944

或者：https://loj.ac/problem/2304  http://uoj.ac/problem/316 NOI2017真题

注：网格区域概率dp+线性递推模板，题解参见：https://blog.csdn.net/ez_yww/article/details/78679459

这个题目算法和复杂度主要在上述两独立部分，这里主要讲dp思路：

设$g_{i,j}$表示长度为$j$，高度为$i$的海域全部是安全的，剩下的部分未知，最大子矩形面积$≤k$的概率之和

设$h_{i,j}$表示长度为$j$，高度为$i+1$的海域中，前$i$行全部是安全的，剩下的未知且$(i+1,j)$是危险的，最大子矩形面积$≤k$的概率之和

设$f_i$为前$i$列最大子矩形面积$≤k$且$(1,i)$为危险格子的概率之和

核心方程：
$$
\begin{aligned} g_{k, 1} &=h_{k,1}=q^{k}(1-q) \\ g_{i, 0} &= h_{i, 0} =1, i \in [1,k) \end{aligned}
$$

$$
\begin{aligned} g_{i, j} &=\sum_{k=0}^{j} h_{i, k} g_{i+1, j-k} \\ h_{i, j} &=\sum_{k=0}^{j-1} h_{i, k} g_{i+1, j-k-1} q^{i}(1-q) \end{aligned} \\
where: j \le\lfloor k/i \rfloor
$$

$$
f_0=1 \\
f_{i}=\sum_{j=0}^{min(k,i-1)} f_{i-j-1} g_{1, j}(1-q)
$$

其暴力时间复杂度为：$\sum_{i=1}^{k}\left\lfloor\frac{k}{i}\right\rfloor^{2}=O\left(k^{2}\right)=O\left(\frac{\pi^2}{6}k^2\right)$

可以使用生成函数优化：
$$
\begin{aligned} A_{i}(x) &=\sum_{j \geq 0} g_{i, j} x^{j} \\ B_{i}(x) &=\sum_{j \geq 0} h_{i, j} x^{j} \\ c_{i} &=q^{i}(1-q) \end{aligned} \\

\begin{aligned} A_{i}(x) &=B_{i}(x) A_{i+1}(x) \\ B_{i}(x) &=c_{i} x A_{i+1}(x) B_{i}(x)+1 \\ B_{i}(x) &=\frac{1}{1-c_{i} x A_{i+1}(x)} \end{aligned}
$$
时间复杂度：$\sum_{i=1}^{k}\left\lfloor\frac{k}{i}\right\rfloor \log \left\lfloor\frac{k}{i}\right\rfloor= O\left(k \log ^{2} k\right)$

使用$O(k^2)$的时间复杂度计算$f[1..k]$，最终答案：
$$
ans=\sum_{i=0}^{k}f_{n-i}g_{1,i}=f_{n+1}/(1-q)
$$
计算$f$的过程本质上是一种只知首项$f_0$的线性递推

关于线性递推部分，参见数学笔记



24.https://www.lydsy.com/JudgeOnline/problem.php?id=1415

注：NOI2005真题，概率dp+贪心+最短路，基础题

25.https://www.lydsy.com/JudgeOnline/problem.php?id=2676

注：wc2013李超题，经典的马尔可夫链模型，二分答案+概率dp+矩阵快速幂

注意求总得分的期望，由于期望的线性性，可以拆分为每个状态点的贡献，因此状态设计为$dp[i][j][k]$表示$i$条生命$j$为当前这一轮如果胜利应该获得的得分(或者如果胜利末尾连续的胜利长度)，当前为第$k$轮的期望

将状态$(i,j)$设计为点(重新编号)，状态转移$(i,j)\rightarrow(min(i+1,q),min(j+1,r))$，概率为$p$，且$(i,j)\rightarrow(i-1,1)，i>1$，概率$1-p$

追加超级源点$tot$，每个点向超级源点连边，边权为这个点如果获胜，则本步的期望对答案的贡献，即$(i,j):j*p$

起始点为状态$(q,1)$，考虑从起始点出发，长度为$0<=k<n$的长度的一条链，链上的边权乘积就是这种情况的概率，只要再乘上此状态的期望，就是条件期望了；前面每个点已经连向$tot$，耗费长度为$1$，故一种情况(假设以概率$p$获得胜利)总长度为$1\le k+1\le n$，因此模型转化为求起点$S$到终点$tot$的长度在$[1,n]$以内的任意有向链边权乘积之和($tot$尚无自环)，只要在$tot$处，追加边权为$1$的自环，即可转化为求$S$到$tot$长度固定为$n$的链路，考虑邻接矩阵的$n$次幂即可

总结：本题最主要的思想是算两次，对每个状态只考虑在此处获胜的条件期望(当然还需要耗费一步)，叠加即得总的期望得分

26.http://codeforces.com/problemset/problem/464/D

注：概率dp+状态空间剪枝优化，详见国家集训队论文《dp的一些优化技巧》

设$f(i,j)$为当前己经有等级为$j$的装备了，再打$i$只怪获得金币的期望
$$
\begin{aligned} 

f(0, j) &=0 \\ 

f(i, j) &=\frac{1}{k} \sum_{x=1}^{j+1} \frac{1}{j+1}(f(i-1, \max (j, x))+\min (j, x))+\frac{k-1}{k} f(i-1, j) \\ &=\frac{1}{k}\left(\frac{j}{j+1} \cdot\left(f(i-1, j)+\frac{j+1}{2}\right)+\frac{1}{j+1} \cdot(f(i-1, j+1)+j)\right)+\frac{k-1}{k} \cdot f(i-1, j)  \\

ans&=f(n,1)

\end{aligned} \\
$$
状态空间剪枝：有价值的状态中$f(i,j)$，$j \le \sqrt{i}$，转移$O(1)$，时空复杂度均为$O(n \sqrt{n})$

27.https://www.lydsy.com/JudgeOnline/problem.php?id=2707

注：相当基础的马尔可夫链模型，有向图上随机游走，求每个点到指定终点的期望步数，$n$比较大，但是数据保证每个强连通分量点数不超过$100$，所以显然就是$tarjan$缩点，之后拓扑排序，每个$scc$去高斯消元即可

28.https://www.lydsy.com/JudgeOnline/problem.php?id=1076

注：概率dp+状压dp，很基础

29.http://codeforces.com/problemset/problem/696/B

注：经典题，有根树随机游走，求每个点dfs序的数学期望

与$codeforces \space 123E$类似的，固定一个点$x$求期望，考虑树上每个点$i$对答案的贡献；

在$dfs$序的问题中，回溯是不计代价的，那么树上有三类点，$i$到根闭路径上的点，有$1$的概率贡献$1$，$i$的开子树上的点，概率为$0$，其他的点，有$1/2$的概率贡献$1$，叠加即可

在回溯计算代价的问题中，从根开始随机$dfs$，搜到固定点$x$就停止，求步数的数学期望；树上有三类点，$i$到根闭路径上的点，有$1$的概率贡献$1$，$i$的开子树上的点，概率为$0$，其他的点，有$1/2$的概率贡献$2$，叠加即得$E(x)=n-sz(x)$

30.https://www.lydsy.com/JudgeOnline/problem.php?id=1444

注：建AC自动机，变量定义为经过每个状态的期望次数，建立方程组高斯消元



31.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=010435 C题

注：概率$dp$，题意：给定一个只含"$H$"和"$R$"的字符串$s$，$H$向左走，$R$向右走，速度相同，当两个不同字母冲突时，$H$有$h$的概率消失，$R$有$r$的概率消失；求在充分长的时间后，有严格$A$个$R$和$B$个$H$存活的概率

- 基本性质
  - 一个$H$，一个$R$，$R$在$H$的左边，这两个字母不可能同时存活
  - 原序列$s$任意一个非空子区间，单独游戏，至少有一个生还
  - 假设最终存在严格$A$个$R$和$B$个$H$存在，设他们的下标分别为$r_1,r_2,\cdots,r_A$和$h_1,h_2,\cdots,h_B$，且分别单调增，则有$h_B<r_1$
  - $h_B+1=r_1$，反证法：如若不然，则$h_B$和$r_1$中间至少存在一个人，构成非空子区间，则至少一人生还，不失一般性，不妨令其为字母$H$，而$h_B$这个下标生还了，该字母$H$显然必定生还，即有$B+1$个$H$生还了，而这显然与假设矛盾
  - 从概率的角度讲，很多同时发生的事件，是可以给定一个顺序，有序发生的，比如下标顺序
  - 从原来序列$s$到最终的$A$个$R$和$B$个$H$的状态，一个个人接连着死去，但无论多么复杂的情况，总是有严格$cnt_h-B$个$H$和$cnt_r-A$个$R$分别以$h$和$r$的概率死去，也就是说对于任何一种合法的情况方案，其发生的概率显然总是相等的，均为$h^{cnt_h-B}$和$r^{cnt_r-A}$，因此我们只需要求合法的方案数$ret$就好了
  - $h_B$不同显然对应不同方案，可以按照$h_B$的取值分类
  - 对于一类，考虑以$h_B$结尾的前缀，和以$r_1$开头的后缀，显然这两部分是独立无关的，因此概率或方案数可以直接相乘
- 算法
  - 过滤掉开头的$H$和结尾的$R$(不做也行)，调整$A$和$B$，计算新的$cnt_h,cnt_r$，特判特殊情况
  - 枚举下标$(i,i+1),i \in [0,n]$，令$f_i$表示$i$这个下标是$H$且必生还，以$i$结尾的前缀严格有$B$个$H$生还，其他字母死光的方案数；令$g_i$表示$i$这个下标是$R$且必生还，以$i$开头的后缀严格有$A$个$R$生还，其他字母死光的方案数；二者对称，只讨论$f$
  - 为求$f$令$dp[i][j]$表示只考虑前$k$个元素($k$为第$i$个$H$下标)，一共严格生还了$B$个$H$且第$i$个$H$必须生还，其他元素全部死光的方案数，该$dp$有参数$B$
  - 转移：考虑前$k$个元素中最后一对(最右边)冲突的字母对，讨论$H$和$R$谁生还
    - $H$生还，$(i,j)\to(i,j-1)$
    - $R$生还，$(i,j)\to(i-1,j)$
    - 故：$dp[i][j]=dp[i-1][j]+dp[i][j-1],i\in[B,cnt_h],j\in[1,a[i]]$，$a[i]$表示第$i$个$H$前面的$R$数量
  - 边界：$\forall i <k\&\&j: dp[i][j]=0$，$dp[k][0]=1$，其余均为$0$
  - 令$id[i]$表示第$i$个$H$的下标，则$f[id[i]]=dp[i][a[i]],i\in [0,cnt_h]$
  - 计算答案：$ans=h^{cnt_h-B}*r^{cnt_r-A}*\sum_{i=0}^nf[i]g[i+1]$
  - 特别当心：注意计算答案时，快速幂指数可能有负要特判
- 正确性：由于边界的控制和转移的范围，转移是正确的
  - 转移的特点：
    - 最右规约，即下标$\in[id[i-1],id[i]]$的$R$没有死光，下标$\in[id[i-2],id[i-1]]$的$R$是不会死的，因为我们每次转移仅考虑最后一对冲突字母对
    - 在某个状态，如果我们转移到了一个非法的状态，这是不要紧的，因为非法状态的方案总是$0$，$dp$值加上$0$，相当于没有这种非法转移
    - 状态$dp[i][j]$当$j>a[i]$是非法状态，注意到最右规约和最左规约是不同的，转移过程中总是保持合法的转移走到的是合法的状态，一个$H$可以被打败，其右侧必无$R$
  - 对于状态$dp[i][j]$，考虑当前第$i$个$H$被打败，显然$(id[i-1],id[i])$之间至少有一个$R$，即$a[i-1]<j$，这是个非法转移，转移到的状态为$dp[i-1][j]$，显然是个非法状态，所以我们的转移是正确的
- 总结：
  - 这样的概率问题是比较复杂的，一般都是要仔细分析一下其中蕴含的性质，然后寻找突破口；在概率意义上，一个问题常常需要分类使用加法原理，我们需要寻找正确的分类依据；对于一类子问题，可能还会涉及一些独立子问题的拆分，使用乘法原理，我们需要想清楚为什么是独立的；然后才能设计合理的状态
  - 考虑转移时，我们需要给复杂的事件序列定个顺序，一个个的考虑；验证转移的正确性，要保证合法的转移，没有重复和遗漏的走到其对应合法的状态；非法的转移，要么就没有转移，要么就走到非法的状态($0$状态)
  - 考虑边界和范围来限制$dp$，精确的定义状态表示和状态的合法性











## 【10】dp优化：分治

1.http://codeforces.com/contest/834/problem/D

2.http://codeforces.com/problemset/problem/868/F



## 【11】其他一些经典例题

1.http://codeforces.com/contest/888/problem/F

2.http://codeforces.com/problemset/problem/930/C

3.http://codeforces.com/problemset/problem/958/C2

注：小模数小段数的关于区间和模和的序列最优切割

4.http://codeforces.com/problemset/problem/1155/D

注：经典的峰形线性dp，允许选择最多一个区间乘给定x的最大连续字段和变种



## 【12】基础dp综合题

1.http://codeforces.com/problemset/problem/864/E

2.http://codeforces.com/problemset/problem/1174/E

注：贪心+dp，考察$gcd$的性质

若$gcd(x,y) <y$则$gcd(x,y) \le y/2$，因此$gcd$会严格下降$log$次

贪心：首元素必为$2^x*3^y,y \in[0,1]$，且每次严格下降$2,3$中的一个

状态表示：$dp[i][x][y]$表示前$i$个元素已经填满且此时$gcd=2^x*3^y$的方案数

3.http://codeforces.com/problemset/problem/1168/C

注：与二进制位$\&$运算有关的$dp$

令$f[i][j]$表示下标$i$能走到的第一个$\ge i$的数值含有$bit_j$的下标

令$g[i][j]$表示下标$>i$的含有$bit_j$的第一个(最小)下标

$f[i][j]=i,a[i]含有bit_j$

$f[i][j]=min(f[g[i][c]][j]),a[i]不含有bit_j,含有bit_c$

回答询问：$x \rightarrow y$

$\exists \space c,st.  f[x][c] \le y,a[y]含有bit_c$

4.http://codeforces.com/problemset/problem/1172/B

注：简单的环状计数dp

用到简单的组合数学结论：将$n$个有标号的元素放入$m$个有标号的集合(左和右，允许为空)中，其方案数为：

$\sum_{k=1}^m\begin{Bmatrix}n \\k\end{Bmatrix}\dbinom{m}{k}k!$，则把$k$个放入$2$个集合为：$(k+1)!$

可以这样理解把这两个集合的分割线看成第$k+1$号元素，加进去一起全排列，方案显然一一对应

令$f[x]$表示把$x$放在弧上特定位置，且把$x$子树上的其他元素铺在这个弧上的不交方案数

显然$f[x]=(|Child(x)|+1)!\prod_{y \in Child(x)}f[y],x!=1$，当$x=1$时，前面阶乘里面不$+1$

实际上，由于邻接表$vi \space V[N]$连的双向边，直接取$sz(V[x])$即可，非根元素本来就多算了一个父亲

$f[1]$表示把$1$放在某个特定位置的方案数，枚举$1$放的具体位置k，$ans=f[1] * n$





## 【13】dp优化：间歇性矩阵快速幂加速转移

1.http://codeforces.com/problemset/problem/954/F

2.http://acm.hdu.edu.cn/showproblem.php?pid=6395



## 【14】dp优化：wqs二分

可以直接认为，当 dp 值只有整数的时候，可以直接用整数进行二分。

学习资料：

https://m.doc88.com/p-949564862405.html

https://blog.csdn.net/CHHNZ/article/details/78827430

http://codeforces.com/blog/entry/49691

https://blog.csdn.net/chhnz/article/details/78846104

https://www.cnblogs.com/CreeperLKF/p/9045491.html



总结：

这一类题目，要求带限制选择严格k个物品，使得目标函数最优化

特点是：目标函数关于物品选择的个数k单调，设为g(k)，g(k)关于k单峰（形状是凸壳）

朴素的dp复杂度太高，如果去掉物品个数那一维的话，往往可以优化到O(n)或者较优的复杂度

二分一个C，表示每选择一个物品的Cost，则目标函数变为f(k)=g(k)-k*C

注意到：f'(k)=g'(k)-C单调，因此可以考虑二分C，dp求出全局无物品个数限制意义下的dp最优值和物品个数(D,X)

用X与题目给的k比较，调整二分的方向；最后获得X=k，ans=D+C*k

当然，对于C，是加入答案，还是从中扣除，根据题目具体情况而定



细节说明：

往往我们优化过的dp，每次求的X是能够取到最优dp值的最大物品个数，

也就是说如果当前物品必取，大于等于不取当前沿用之前最值，就更新，然后与k比较(>=k为一边方向)

这样做的根据是：我们总是找使得x>=k成立的最大或最小的C(C如果是小数，不必十分精确)

每次只要符合这个要求，那么我们记录二元pair(dp最优值，物品个数)

设想一下，比我们找的C次一点的C'，会使得h(C')=x' < k成立，那么[h(C')+1,h(C)]这一段C相同，因而dp最优值相同

而题目的k必然在其中的，因此不影响答案求法的正确性




题目：

1.http://codeforces.com/problemset/problem/958/E2

2.http://codeforces.com/problemset/problem/739/E

3.https://www.lydsy.com/JudgeOnline/problem.php?id=2654

4.http://poj.org/problem?id=1160

5.https://www.lydsy.com/JudgeOnline/problem.php?id=5252

6.https://www.lydsy.com/JudgeOnline/problem.php?id=5311

7.http://codeforces.com/gym/101981/attachments B题

8.http://uoj.ac/problem/240





## 【15】计数dp：映射原理+简单容斥

1.http://codeforces.com/problemset/problem/1093/F

2.http://codeforces.com/group/aUVPeyEnI2/contest/243687 C

注：烷烃同分异构体(500个点以内)，无根树计数dp





##【16】与自动机有关的dp：隐藏自动机

1.http://codeforces.com/problemset/problem/1142/D

注：自动机思想+dp计数，统计一类子串数量

题目会先定义一个多重集合或者串空间，往往元素数量巨大或者无穷多，而*<u>自动机的本质功能就是分类表示与识别，用有限的状态表示无限的元素</u>*，我们需要分析空间元素生成的规则，从而提取特征，设计状态：

本题中，$1-9$在集合里面，一个元素$x \in S，rank(x)=c \pmod{11}$，则$x$可以扩展出$10x+i,i \in [0,min(c,10))$，也就是说最后可以加一个严格小于自己排名的数字

**这个空间有以下基本性质：**

- 单调性，若一个数字串$s \in S$，则$s$的任何一个前缀均$ \in S$；若$s \notin S$，则$s+t \notin S,\forall t$
- 若$s \in S$，$p[i]$为$s$的任一个非空前缀，则$rank(p[i])\%11>s[i+1]，\forall \space i \in [1,n-1]$

第一个性质告诉我们，只要对每个下标$i \in [1,n]$，求以此为起点的可延续的最长合法长度$len(i)$即可

第二个性质告诉我们，前缀串的$rank\%11$与后面可加的数字有关，这表明$rank\%11$是状态设计的依据，而后面可以加的数字是某个状态可选的转移依据

我们追加$0$元素到集合$S$中，$rank(0)=0$，所有元素按照$rank \% 11$分类，以此为据设立自动上的$11$个状态节点，再加一个空节点$Null$，是在自动机上运行串的起点状态；每个状态的可选转移按上述，我们需要求出状态$x$在$c$方向，转移到的状态$y$

画一个图，$0-10$元素，为第一行(共$11$个元素)，然后第二行为第一行元素的按序扩展序列，$0$扩展$0$个，$1$扩展$1$个，$\dots$，$10$扩展$10$个，第二行共$55$个元素，且是升序的紧接第一行元素的，注意此处$10$多出现了一次，但是我们不再图中删除，在公式中$-1$即可

将第一行$11$个元素看成一组，跳过第二行的$10$，以后每$11$个元素看成一组，可以发现，每组第$0$个元素$rank$是$11$的倍数，因此一组和上面第一行的规律相似，我们只需要前两行数据，因为我们要计算转移$(x,c)=y$，这里的$x \in [0,10]$，是第一行的元素，那么$[0,x-1]$这些元素扩展完毕了，共$x(x-1)/2$个，而这个转移是$x$的第$c$个转移($[0,c]$转移完毕)，共$c+1$个，加之得到$y$第二行的排名，减去开头的多余的一个$10$，加上第一行的$10$个元素，则总排名为$y=x(x-1)/2+c+10 \pmod{11}$，这个函数记作$nxt(x,c)$

**下面的$dp$是很自然的：**

令$dp[i][j]$表示在自动机上的状态$j$，从串的下标$i$开始向右匹配的最长匹配长度

显然，如果$j  \le s[i]-'0'$，则一步都走不出去，$dp$值为$0$，我们忽略这种转移

而$i \in [1,n]$，$j>s[i]-'0'$，则$j$这个状态存在转移方向$s[i]-'0'$，即至少可以走一步，走了一步之后$j$走到了新状态$nxt(j,s[i]-'0')$，故：$dp[i][j]=dp[i+1][nxt(j,s[i]-'0')]+1$

计算答案时，每个下标从$Null$状态开始在自动机上走：

$ans=\sum_{i=1}^ndp[i][Null]=\sum_{i=1}^n(dp[i+1][s[i]-'0']+1)$

**总结**

对某个状态空间构造自动机，其关键就在于空间元素扩展过程中有什么***变化的且有穷的属性***，可以考虑作为状态设计依据

## 

## 【17】与子序列有关的dp

1.http://codeforces.com/problemset/problem/1096/D



## 【18】动态dp

### 参考资料

https://www.cnblogs.com/YoungNeal/p/10360291.html

http://immortalco.blog.uoj.ac/blog/2625

https://www.luogu.org/blog/gkxx-is-here/what-the-hell-is-ddp （洛谷日报 #130）

https://www.luogu.org/problemnew/solution/P4719

### 动态dp

1、用树剖实现复杂度是 $O(nlog_2^2n*矩乘复杂度)$

2、LCT实现复杂度是 $O(nlog_2n)$，常数比较大

只需要用到其中的access操作。

3、全局平衡二叉树实现复杂度是 $O(nlog_2n)$，常数非常优秀，可以替代一类静态树上的路径问题。

### 题目

https://www.luogu.org/problemnew/show/P4719

- 写出dp转移
- 修改结点价值，维护dp值
  - 序列问题可以用数据结构维护矩阵乘法
  - 树上问题需要先树剖，维护和重儿子之间的关系，修改一个点的时候，它所在重链顶端节点的父亲的矩阵会改变，需要一直跳上去更新。只维护重链顶端的节点的真实dp值，其他节点的dp值均需要在线查询。

https://www.lydsy.com/JudgeOnline/problem.php?id=4712

https://www.lydsy.com/JudgeOnline/problem.php?id=5210

http://uoj.ac/problem/441

https://www.luogu.org/problemnew/show/P4751

https://www.lydsy.com/JudgeOnline/problem.php?id=5287

https://www.lydsy.com/JudgeOnline/problem.php?id=4732

https://www.lydsy.com/JudgeOnline/problem.php?id=4911


##【19】括号序dp/扫描线式线性插头dp

1.http://codeforces.com/problemset/problem/626/F

注：经典的线性插头dp或者说括号序dp

**总结**

此种$dp$常设状态表示$f[i][j][\dots]$表示考虑前$i$个元素，有$j$个带匹配插头，且满足一些其他限制的答案

状态转移常有以下几类，分类讨论即可：

- 新建一个带匹配插头$\rightarrow f[i+1][j+1],*1$

- 匹配一个之前的带匹配插头$\rightarrow f[i+1][j-1],*j$

- 此元素作为中间元素考虑/不选$\rightarrow f[i+1][j],*1/*j/\dots$

- 此元素单独构成一个自闭的自插头(新建且立刻与自己匹配)$\rightarrow f[i+1][j],*1$

- 先与之前的某个插头匹配，然后再新建一个插头$\rightarrow f[i+1][j],*j$

当然，转移还受其他约束限制影响，一般答案为$f[n][0][\dots]$

2.http://codeforces.com/problemset/problem/466/D

注：与上题相似







## 【20】dp组合与嵌套

1.http://codeforces.com/problemset/problem/1158/F

注：难题，当权值比较小的时候，用状压dp；权值比较大，用下标转移的普通dp

**结论：判定一个序列(字符集为$[1,c]$)包含长度为$p$的任何一个同字符集的序列以之为子序列，方法如下：**

称上述最大的$p$为序列的密度，显然有单调性，即对$\forall i \le p$依然满足条件

每次寻找最小的下标$j$，使得序列前缀$pre[j]$满足：包含$\forall i \in [1,c]$至少一次，且包含字符$a[j]$严格一次，该前缀称为一个块，删之重复操作，能够构造的最大块个数即是密度$p$

证明：原序列为$a$，删除一个块前缀为序列$a'$，只要证明$a$密度为$p$，等价于$a'$密度为$p-1$

必要性显然，充分性：$a$包含任何一个长度为$p$的字符集为$c$的子序列，那么必然包含长度为$p$，且以字符$a[j]$开头的任何子序列，其中$j$为第一个块终点且我们取(如果不取，可以调整到取)，而第一个块中不包含其他位置的$a[j]$字符，那么取这个$a[j]$，在去掉第一个块前缀之后$a'$即包含任何长度为$p-1$的字符集为$c$的子序列，命题得证

注意此结论与序列自动机的性质有关，参见字符串相关词条，含证明

**题解：**令$dp[i][j]$表示在$[1,j]$中取了的子序列里，构成$i$个块，第$i$个块以下标$j$结尾且$j$必取的方案数或者子序列个数，下面有两种不同的辅助$dp$获得上述$dp$值：

*$状压dp$*

令$u[i][j][mask]$表示考虑$[1,i]$中选了的子序列里包含$j$个块，且第$j+1$个块可能残缺，其包含字符的情况为二进制$mask$
$$
mask>0,a[i] \in mask: \space u[i][j][mask]=2u[i-1][j][mask]+u[i-1][j][mask-2^{a[i]-1}] \\
mask>0,a[i] \notin mask: \space u[i][j][mask]=u[i-1][j][mask] \\
mask=0: \space u[i][j][0]=u[i-1][j][0]+dp[j][i] \\
dp[j][i]=u[i-1][j-1][2^c-1-2^{a[i]-1}] \\
dp[0][0]=u[0][0][0]=1 \\
时间复杂度O(nK2^c),K=n/c
$$
普通$dp$

令$num[i][j]$表示$[i,j]$中下标$j$必取，且取出一个子序列构成恰好一个块的方案数；令$cnt_x[i][j]$表示$[i,j]$中字符$x$出现的次数，下面意思是说除了字符$a[j]$，其他字符至少取一个，而字符$a[j]$取且仅取下标$j$
$$
num[i][j]=\prod_{x=1,x\ne a[j]}^c (2^{cnt_x[i][j]}-1) \\
dp[i][j]=\sum_{t=0}^{i-1}dp[i-1][t]*num[t+1][j] \\
dp[0][0]=1 \\
时间复杂度O(n^2K)
$$
计算答案
$$
f[t]=\sum_{i=1}^n dp[t][i]*2^{n-i},t \in [1,K] \\
ans[t]=f[t]-f[t+1], t \in [0,n] \\
总体时间复杂度O(nKmin(n,2^c)) \ge O(n^3/logn),c以logn为界
$$
**总结：**

这是一种序列的切割$dp$，但是一个块中方案数又可以和权值范围有关系，那么就可以用这种经典的组合$dp$

有时候，$dp$一步很难表示出答案或者转移，需要很多的辅助量，可能需要$dp$嵌套，当有多个量纠缠在一起时，我们要充分挖掘之间的联系，用它们相互表示









# 6.博弈论，贪心和构造

##【1】博弈论基础

1.http://acm.hdu.edu.cn/showproblem.php?pid=2149

2.http://acm.hdu.edu.cn/showproblem.php?pid=3980

3.http://acm.hdu.edu.cn/showproblem.php?pid=3595

4.http://acm.hdu.edu.cn/showproblem.php?pid=1846

5.http://acm.hdu.edu.cn/showproblem.php?pid=5754

6.http://acm.hdu.edu.cn/showproblem.php?pid=3032

7.http://acm.hdu.edu.cn/showproblem.php?pid=5011

8.http://acm.hdu.edu.cn/showproblem.php?pid=1730

9.http://acm.hdu.edu.cn/showproblem.php?pid=1525

10.http://acm.hdu.edu.cn/showproblem.php?pid=2516

11.http://acm.hdu.edu.cn/showproblem.php?pid=1517

12.http://acm.hdu.edu.cn/showproblem.php?pid=4387

13.http://acm.hdu.edu.cn/showproblem.php?pid=1907

14.http://codeforces.com/problemset/problem/832/A

15.http://codeforces.com/problemset/problem/812/E

16.http://codeforces.com/problemset/problem/794/E

17.http://codeforces.com/problemset/problem/786/A

18.http://codeforces.com/problemset/problem/768/E

19.http://codeforces.com/problemset/problem/731/E

20.http://www.lydsy.com/JudgeOnline/problem.php?id=1443

21.http://codeforces.com/problemset/problem/917/B

22.http://codeforces.com/problemset/problem/859/C

23.https://nanti.jisuanke.com/t/31442

24.http://codeforces.com/problemset/problem/36/D

25.http://codeforces.com/gym/101981/attachments A题

26.https://codeforces.com/problemset/problem/1099/F

注：博弈+简单贪心+树dp+线段树

27.https://codeforces.com/problemset/problem/317/D

注：取x同时删除x^k(k>=1)，幂次不交链游戏和

28.https://codeforces.com/problemset/problem/1100/D

注：鸽巢原理+棋盘逼近问题(控制一个对象，将其他对象逼近角落)

29.https://codeforces.com/problemset/problem/38/F

注：既有必胜又有得分的题目，游戏状态状态可以表示成类似的三元组(op,x,y),

op==1表示此状态下先手必胜，-1必败，0平局或者无法确定；x当前先手得分，y当前后手得分；

那么每个游戏状态在转移的时候，相当于在所有后续游戏状态调整后的评价中，求最小值；

最小值bool逻辑按照(1<,3>,2<),123为三个分量，<表示越小越好；

当前游戏状态评价应该为此最小值，第一维取相反数，二三维交换；

30.https://codeforces.com/problemset/problem/154/D

注：分类讨论，对称思想，nim游戏扩展

31.https://codeforces.com/problemset/problem/273/E

注：sg函数取值为[0,2]，sg函数分布为块状，块个数很少，未得到证明

博弈必胜计数题，一个个生成块，博弈+二分+简单dp

32.https://codeforces.com/problemset/problem/138/D

注：实现小技巧，当n行m列菱形网格(黑白染色，同色格子)旋转时，可认为坐标变换为(i,j)->(i+j,j-i+n)，类比于切比雪夫坐标变换

33.https://codeforces.com/problemset/problem/1110/G

注：等价转换，分类讨论，探索充要条件，构造性

34.https://codeforces.com/problemset/problem/98/E

注：带欺骗的博弈概率dp，考虑玩家的心理决策表(行为先手是否欺骗，列为后手是否相信)，存储先手获胜概率，每个元素按照对应的概率分布列分类讨论；一个游戏状态先手最优策略为是否欺骗的线性组合，设选择欺骗的概率为p，求最值

35.http://acm.hdu.edu.cn/showproblem.php?pid=3537

注：一种硬币游戏，翻动不超过三枚硬币

36.https://codeforces.com/problemset/problem/142/D

注：经典的nimk游戏，注意平局细节

37.https://codeforces.com/problemset/problem/1076/G

注：博弈论+线段树+函数变换复合/嵌套(结合律)+简单dp

首先分析某个位置i的NP态特性，对a[i]分奇偶，且仅与后面连续m个NP状态有关，看成是关于长度为m的二进制串的状态变换；此处可优化为：注意到二进制空间中，每个状态可以分成很多类，每类仅与最靠近的P态位置有关；令h[i]表示传入二进制状态s最靠近的P态位置为i时，变换后此位置变为多少；以h代替串s本身，h[0..m]，其中h[m]表示串s在0..m-1位置无0，h易可合并；查询时，求出区间合并后的总变换，传入s=全1串，表示禁止转移，相当于取出h[m]；


38.https://www.lydsy.com/JudgeOnline/problem.php?id=5326

39.http://codeforces.com/gym/102220/problem/F

注：有向图博弈扩展+spfa

经典的有向图(有自环，无重边)博弈扩展，$NP$状态定理推广，$s_{i,j}$表示$j$这个人在$i$这个点时游戏状态，$0$为待定或者平局，$1$表示必胜，$-1$表示必败，注意以上定义都是针对$j$这个人所在阵营；从出度为$0$的点$u$且人为任意$p$的游戏状态$(u,p)$出发，利用$spfa$递推；对每个队列中待扩展状态$(u,i)$，先计算上一个人$j$，弄清楚$j$支持哪一方，即$j$的目的，以及$j$是否支持$i$所在方(一个$int$量$c \in \{1,-1\}$)，则用判断式$c==s_{u,i}$可以表示$j$这个人是否可以在某个游戏状态通过选择一步转移到状态$(u,i)$达到自己的目的(即支持$i$所在方，且状态$(u,i)$中$i$所在方必胜；反对$i$所在方，且状态$(u,i)$中$i$所在方必败)，如果此状态没访问过，那么$s_{v,j}=j$是否支持己方，入队；$c==-s_{u,i}$，则应该使得每个前驱状态出度减$1$，无可奈何的状态(出度减为$0$)则只有违背$j$的意愿$s_{v,j}=j$是否支持己方的相反数，入队；这两种情况入队，其他情况表示出现平局，不对其他状态产生有效影响，注意到每种状态最多入队两次(因为上述每种情况最多入队一次)，时间复杂度为$O(n+m)$

40.https://www.luogu.org/problemnew/show/P4643



41.http://poj.org/problem?id=2931

注：经典的不平等博弈，$surreal \space number$的应用，参见国家集训队论文2019例题

$bush$游戏的基础版本的特殊情形，不需要实际求出游戏数，只要分析出结论即可







【the Shannon switching game】



##【2】贪心


指定题目：

1.http://codeforces.com/problemset/problem/835/B

2.http://codeforces.com/problemset/problem/830/A

3.http://codeforces.com/problemset/problem/827/B

4.http://codeforces.com/problemset/problem/773/C

5.http://codeforces.com/problemset/problem/796/F

6.http://codeforces.com/problemset/problem/769/B

7.http://codeforces.com/problemset/problem/758/E

8.http://codeforces.com/problemset/problem/754/D

9.http://codeforces.com/problemset/problem/748/E

10.http://codeforces.com/problemset/problem/735/C

11.http://codeforces.com/problemset/problem/732/E

12.http://codeforces.com/problemset/problem/721/D

13.http://codeforces.com/problemset/problem/908/F

14.http://codeforces.com/problemset/problem/917/A

15.http://codeforces.com/problemset/problem/922/D

16.http://codeforces.com/problemset/problem/946/E

注意：比较函数要满足传递性,反对称性，反自反性

17.http://codeforces.com/problemset/problem/865/D

注：替换式优先队列贪心

18.http://codeforces.com/problemset/problem/962/E

注：经典题目：一维点的连通性/一维最小点归属问题

19.http://acm.hdu.edu.cn/showproblem.php?pid=6299

注：与括号序列及其最简二元组表示有关的贪心

20.http://codeforces.com/problemset/problem/1031/F

注：经典问题，一维2n个点，最小距离和匹配贪心

21.https://vjudge.net/contest/274500#problem/D

22.http://codeforces.com/problemset/problem/1082/E

注：最大连续字段和变种贪心

23.https://cn.vjudge.net/contest/274676#problem/G

注：二进制按位递归式贪心，a[]进行sort之后，构成天然01字典树

24.http://codeforces.com/problemset/problem/1092/E

注：经典问题：森林连边构造树，最小化直径；

与直径有关的贪心，利用直径性质可以证明：

树上中心，在直径中点；森林构造成菊花树林，本题是树上中心模板题

25.http://codeforces.com/contest/1090/problem/L

26.http://codeforces.com/problemset/problem/1088/E

注：最大连续子段和树上推广，同时计数(最大数量)

27.http://codeforces.com/problemset/problem/1088/F

注：题目有个地方没有强调，每个非最小值点有且仅有一个点权比其小的邻接点

证明：分三步证明

1)先把贡献拆成边的贡献式，也就是说，问题本质相当于求完全图某种最小生成树权值

2)证明非最小值点负责连一条出边，且这个连边操作，点与点之间是无序的

3)证明每个点u必然与自己祖先的某个点v相连，而不会是非祖先点，这是因为可以很容易调整为取v=lca(u,v)，公式具有单调性

技巧：当树上倍增被卡空间时(空间nlogn)，可以不开倍增数组，dfs时维护关于深度(根深度为0)的人工栈，里面维护根到当前所访问点的路径(当前路径，存储点编号)

28.http://codeforces.com/problemset/problem/1082/E

29.http://codeforces.com/problemset/problem/1091/F

30.http://codeforces.com/problemset/problem/1095/F

注：最小生成树变种贪心，只需要考虑除读入边之外的一些关键边，简单的调整法就可以证明

31.http://codeforces.com/problemset/problem/1097/C

注：与括号序列及其最简二元组表示有关的贪心

32.http://codeforces.com/problemset/problem/1097/E

注：与LIS树有关的贪心，关于LIS树是说：

**$LIS$树**

给定一个排列，$1-n$中任何一个数对应于树上一个节点，根为$0$元素，根到节点$i$的有序路径表示以$i$这个值为结尾的字典序最小的最长$LIS$方案，其构造方法如下：

维护一个单调迭代数组(是这样一个数据结构，不妨设单调递增，支持末端插入元素的动态数组，单点替换，修改操作不影响数组单调性)，$s[1..cnt]$，其中某个时刻$T$时，插入元素$x$，二分查找$s$中第一个大于$x$的数的下标$i$，$s[i]$由$y$替换为$x(y>x)$表示以值$x$结尾的$LIS$长度为$i$，且存在一个字典序最小的方案，方案中$x$的前驱元素应该是此时的$s[i-1]$，利用前驱关系构建出来的显然是一棵有序树(儿子们相对有序)，元素$y$被$x$替代，表明$x$和$y$在同一层，且$x$在$y$的右侧；这个数组在某个时刻的数学意义是这棵树的右侧投影节点编号序列，这棵树的深度是整个排列的$LIS$长度，同层元素递减；

这个结构可以很方便的证明排列的最小递增子序列的切割定理，一个排列最少可以分成$k$个单调递减的子序列，其中$k$为最长上升序列的长度；这是因为，只要把树上每层的元素拿出来，就是一个方案，这表明$k$至多是$LIS$长度，而树上深度最大的叶子节点，显然要至少深度个递减序列覆盖，所以$k$至少是$LIS$长度，故$k=len(LIS)$得证；

这个题目是说：如果对于长度为$n$的任意排列，只需要最多$k$个单调切割子序列就足够了，那么给定一个长度为$n$的排列，构造不多于$k$的切割方案，在此意义下最耗费资源的排列显然为1   3 2   6 5 4   10 9 8 7 ... 需要寻找最小的$k$使得$k*(k+1)/2 \ge n$，这就是答案。

这个特殊排列的最少单调切割序列个数确实是$k$，这是因为：我们假设$n=k*(k+1)/2$，不够可以补全，我们观察最后一个递减连续序列，长度必然为$k$，如果方案中有这个递减序列存在，那么可以用数学归纳法证明更小规模的问题(递降直到没有)；如果不存在，那么容易看到最后一个递减连续序列至少需要$k$个单调序列覆盖，也就是答案$\ge k$，而整个排列确实$k$个单调序列就足够了，因为可以取这个$k$个递减序列1,3 2，6 5 4,10 9 8 7...；所以上述不等式：答案$ \ge k$可以取到等号；

一个比较优的但未必是最优的单调切割方案(可以递增可以递减)，可以是：当一个排列的$LIS$长度$>k$，则去掉树上的一条最长根-叶子链，然后转化为子问题递归解决(相当于$n$至少减少$k$，$k$至少减少$1$，因为$n' \le (k-1)*k/2$)；否则，直接利用每层切割方案，构造严格深度个($\le k$个)递减序列。注意到这样构造出来的方案，具有不多于$k$个切割子序列。

由于其结构有一定性质，可以在数据结构中结合$LIS$经典问题；$LIS$树的构造有模板($LIS_T$)。



**$LIS$树扩展**

对每个节点$u$，假设深度为$d$，在$d-1$层中二分第一个严格小于$u$的节点$v$，连接红有向边$u \rightarrow v$

这表示节点$u$每次可以选择一个父节点$t \in [v,p[u]]$，向上走过去，直到走到根，$reverse$可以对应任何以$u$结尾的$LIS$方案，当然每次选择对应最左边的$v$，可以构造字典序最大的方案

此方法可以轻松解决$LIS$相关计数等问题，在建树之后只需要$O(n)$预处理，即可获知$f[i]$以$i$结尾的$LIS$方案数，就可以不用一些数据结构去优化计数$dp$的转移了

也可以在此基础上用线段树优化建图，但目前尚未发现相关经典的应用





33.http://codeforces.com/problemset/problem/1119/E

注：多带一型贪心，指的是每次取k个相等的数x，再多带一个<=x的数，这种贪心就是记录剩余几个单独的没被匹配的，每次扫描到一种数之后，优先匹配这些剩余的，然后自我匹配，再更新数量，维护剩余数

34.https://www.lydsy.com/JudgeOnline/problem.php?id=5289

35.http://codeforces.com/problemset/problem/125/D

注：鸽巢原理+贪心构造，把没有相同元素的序列拆分为两个等差数列

36.http://codeforces.com/group/aUVPeyEnI2/contest/243687 F

37.http://codeforces.com/problemset/problem/650/D

注：LIS基本性质分析+分类讨论，半动态单调修改LIS：如果修改某个下标的值，修改独立，那么求新的LIS长度

本题涉及：判断下标$i$，是否可能存在于一个$LIS$方案中，记为$ok[i]$；判断下标$i$，是否被所有$LIS$方案包含，记为$yes[i]$

令$f[i]$表示以下标$i$结尾的$LIS$长度，$g[i]$表示以下标$i$开头的$LIS$长度，则$ok[i] = (f[i]+g[i]-1==L)$，其中$L$为整个序列的$LIS$长度

令$yes_l[i]$表示是否不存在下标$j<i$，满足$ok[j]\&\&a[j] \ge a[i]$，$yes_r[i]$表示是否不存在下标$j>i$，满足$ok[j]\&\&a[j] \le a[i]$，则$yes[i]=yes_l[i]\&yes_r[i]$，采用类似于前缀和/扫描线的算法维护最大值或者最小值即可$O(n)$预处理

本题分析：单点修改($a[i]\rightarrow b[i]$)之后，将所有子序列分类：是否包含下标$i$

若包含$i$，则最大长度为：$f'[i]+g'[i]-1$，注意这里数组是取代之后的

若不包含$i$，则相当于在原数组$a[]$中去掉下标$i$，讨论下标$i$是否是所有原$LIS$必经的：若$yes[i]$，则去掉$i$，答案会是$L-1$；否则，答案不变$L$；因此，此类答案为$L-yes[i]$

**$LIS$其他性质**

对任意$i \in [1,n]$，均满足：任取一个$LIS$方案$e$，$a[i]$在$e$中的排名相同









##【3】构造

1.http://codeforces.com/problemset/problem/643/B

2.http://codeforces.com/problemset/problem/708/B

3.http://codeforces.com/problemset/problem/721/D

4.http://codeforces.com/problemset/problem/730/B

5.http://codeforces.com/problemset/problem/740/B

6.http://codeforces.com/problemset/problem/746/G

7.http://codeforces.com/problemset/problem/715/D

8.http://codeforces.com/problemset/problem/804/E

9.http://codeforces.com/problemset/problem/835/E

10.http://codeforces.com/problemset/problem/665/D

11.http://codeforces.com/problemset/problem/638/A

12.http://codeforces.com/problemset/problem/644/A

13.http://codeforces.com/problemset/problem/593/C

14.http://codeforces.com/problemset/problem/549/B

15.http://codeforces.com/problemset/problem/584/E

16.http://codeforces.com/problemset/problem/906/B

17.http://codeforces.com/problemset/problem/936/C

18.http://codeforces.com/problemset/problem/959/C

19.http://codeforces.com/problemset/problem/990/D

原图与补图联通块数目限制的邻接矩阵构造

20.http://codeforces.com/problemset/problem/990/F

流量守恒无向图的边权构造

21.http://codeforces.com/problemset/problem/959/D

两两互质的带条件数组的构造

22.http://codeforces.com/problemset/problem/960/C

条件子序列计数相关构造

23.http://codeforces.com/problemset/problem/1016/D

注：化归，独立考虑bit，极大子矩形的应用（尽可能简单自由）


24.http://acm.hdu.edu.cn/showproblem.php?pid=6300

25.https://vjudge.net/contest/274500#problem/D

26.https://vjudge.net/contest/274500#problem/F

27.http://codeforces.com/gym/101981/attachments K题

28.https://ac.nowcoder.com/acm/contest/296/B

注：与括号序列与栈有关的构造题

29.http://codeforces.com/problemset/problem/1090/E

注：跳马构造问题，棋盘马圈

30.http://codeforces.com/contest/1090/problem/D

31.http://codeforces.com/contest/1090/problem/C

注：带一定分析和代码量的，操作构造题；需要证明存在性和正确性

32.http://codeforces.com/problemset/problem/1088/D

注：常规异或构造交互题，按位构造

33.http://codeforces.com/problemset/problem/1088/C

34.https://codeforces.com/problemset/problem/1098/C

注：先构造，后调整，构造一棵树，所有节点深度和严格为s，然后使得宽度(节点最大儿子数目)最小

35.https://codeforces.com/problemset/problem/1133/F2

注：定点定度生成树构造，先构造指定点取最小度的生成树(维护父亲数组)，遍历与该点直接相连的点，根据需要修改父亲来调整，显然任意调整的中间状态任意时刻仍然为生成树

36.http://codeforces.com/group/aUVPeyEnI2/contest/243686 K题

注：正则图构造+正则二分图构造

37.http://codeforces.com/group/aUVPeyEnI2/contest/243687 J题







##【4】博弈深入：



广义地理游戏

Generalized geography

PSPACE-complete problems



学习链接：维基百科

https://en.wikipedia.org/wiki/Generalized_geography?tdsourcetag=s_pctim_aiomsg

https://en.wikipedia.org/wiki/Category:PSPACE-complete_problems

https://en.wikipedia.org/wiki/List_of_PSPACE-complete_problems













# 7.数学

【1】初等数论基础：具体数学第4章

【2】组合数学：具体数学第6章

【3】扩展欧几里得/费马小定理/欧拉定理/逆元/筛法/卢卡斯定理

一次同余方程$ax=b\pmod{p}$，有解条件：$gcd(a,p)|b$

设$a,b,p$约去$gcd(a,p)$为$a',b',p'$，则：$a'x=b'\pmod{p'},a'\perp p'$

故得到特解：$x_0=a'^{-1}b'\pmod{p'}$，显然通解$x\pmod{p}$有$gcd(a,p)$种

【4】计算几何：各种基础知识



指定题目：

1.http://codeforces.com/problemset/problem/758/F

2.http://codeforces.com/problemset/problem/756/F

3.http://codeforces.com/problemset/problem/717/A

4.http://codeforces.com/problemset/problem/707/C

5.http://codeforces.com/problemset/problem/710/D

6.http://www.lydsy.com/JudgeOnline/problem.php?id=4002

7.http://www.lydsy.com/JudgeOnline/problem.php?id=1856


【4】积性函数与线性筛法

【5】容斥原理

【6】二项式反演/莫比乌斯函数反演变换

【7】中国剩余定理与扩展/裴蜀定理/威尔逊定理/鸽巢原理/其他一些简单定理（书）

【8】群论基础与$Polya$计数法定理，$bunside$引理



【9】离散对数与原根

[在线求原根](http://www.bluetulip.org/2014/programs/primitive.html?inputbox=6&resultbox=3+has+1+primitive+roots%2C+and+they+are+and+2.) [维基百科：原根](https://en.wikipedia.org/wiki/Primitive_root_modulo_n)

- 关于原根存在的充要条件：

  - 原根存在，则$m=1,2,4,p^a,2p^a$，其中$p$为奇质数且$a \ge 1$
  - $m \ge 3$原根存在，$x^2=1\pmod{p}$存在两解(模$p$意义下)
  - $m \ge 3$，$[1,m]$中与$m$互质的数的乘积模$m$为$-1$有原根，为$1$则无原根

  $$
  \prod_{k=1 \atop \mathrm{ged}(k, m)=1}^{m} k 
  \equiv\left\{\begin{aligned}-1 &(\bmod m) \space ,m\in [1,2,4,p^e,2p^e],p为奇质数 \\ 1 &(\bmod m),否则 \end{aligned}\right.
  $$

  上述结论在模$m^2$意义下未必成立，若成立则$m$为$Wilson \space  numbers$

  上述结论可推广到***任意有限交换群***，群中所有元素的乘积等于单位元或者一个阶为$2$的元素[维基百科](https://en.wikipedia.org/wiki/Wilson%27s_theorem#Gauss.27s_generalization)

  关于[威尔逊商数](https://en.wikipedia.org/wiki/Wilson_quotient)，其同余递推式与伯努利数有关
  $$
  \begin{array}{l}{W(p) \equiv B_{2(p-1)}-B_{p-1}\pmod{p}} \\ {p-1+p t W(p) \equiv p B_{t(p-1)} \pmod{p^2}}\end{array}
  $$

- 求原根算法$O(glog^2p)$

- $BSGS$及其扩展求离散对数$a^x=b\pmod{p}$即$x=log_ab\pmod{\phi(b)}$,$p$未必与$a$互质

  其算法实质是分块思想，扩展时两边同时消因子，复杂度$O(\sqrt{p})$

- 解高次同余方程$x^a=b\pmod{p}$，$p$为质数
  $$
  log_g^x=log_{g^a}x^a=log_{g^a}b\pmod{\phi(p)} \\
  alog_g^x=log_g^b\pmod{\phi(p)}
  $$
转化为第二种情形，即$(g^a)^x=b\pmod{p}$
  
  如果要求所有$[0,p)$中的解，最好转化后用$exgcd$解普通同余方程或者求逆元，得到一个最小特解$log_g^x=a'^{-1}(log_g^b)'=y_0\pmod{\phi(p)'}$，则通解显然为：$y_0+k\phi(p)',k\in[some \space range]$
  
  通解在$\pmod{\phi(p)}$意义下有$gcd(a,\phi(p))$种，这与原高次同余方程的解$\pmod{p}$显然一一对应
  
- 解高次同余方程$x^a=b\pmod{p}$，$p\in Z^+$

  - 特判$p=1$，特判$a=0$
  - 将$p$分解质因子，要求$2$的指数不超过$2$，否则将因为没有原根，而报无解
  - 对每个$p^k$单独考虑，化为模数为质数的幂次的情况，最后中国剩余定理$crt$合并
  - 将$b$规范化($b \in [0,p^k)$)，然后分解为$b=b'p^{cnt}$，其中$p^{cnt}||b$
    - $cnt \ge k$，即$p^k|b$，此时$b$必为$0$，特判之
    - $cnt>0$，即$gcd(b,p^k)>1$，方程化为：$x^a/p^{cnt}=\frac{b}{p^{cnt}}\pmod{p^{k-cnt}}$
      - 特判$a \not|cnt$，此种情况认为无解
      - 化为：$(\frac{x}{p^{cnt/a}})^a=\frac{b}{p^{cnt}}\pmod{p^{k-cnt}}$，转化为互质情形
    - $cnt=0$，即互质情形，与上一个知识点类似，即当$p$为质数时
  - 常常构造最小非负整数解($crt$直接合并)，求解$\in[0,p)$个数，求所有解等
  - 求解个数，可以根据$crt$证明解的一一对应，即简单的利用乘法原理即可
  - 模板支持：$a \ge 0,1\le p<10^{12}$，分解后每类均有原根

- 原根的性质：

  - 数量：$\phi(\phi(p))$
  - 可相互表示：若$g$为原根，则$g^k$亦为原根，其中$k\perp\phi(p)$
  - 若$g$是质数$p$的一个原根，则$p^k$原根为：
    - $g+p$，当$g^{p-1}=1\pmod{p^2}$
    - $g$，否则
  - 若$g$是$p^k$的一个原根，则$2p^k$原根为：
    - $g$和$g+p^k$其中任意一个奇数
  - 若质数$p!=3$，则其所有原根之积$ret=1\pmod{p}$
  - $\forall$质数$p$，其所有原根之和$ret=\mu(p-1)\pmod{p}$
- 注意点：

  - 不确定是否不同余$0$，就要讨论及特判
  - 注意在数学上$0^0=1$，故同余方程$a^x=b\pmod{p}$，当$a=b=0$时，注意最小非负整数解$x_0=[p==1]\oplus1$



【10】二次剩余与$n$次剩余

【11】生成函数与狄利克雷卷积

狄利克雷卷积本质：无穷高维普通卷积$fft$

【12】类欧几里得算法

【13】高斯消元法的应用：解线性方程/异或方程组/数学期望问题

【14】几类重要的数列

【15】线性规划问题

【16】组合恒等式的推导与论证

【17】几类积性函数的求和方法/杜教筛（有论文）

【18】几个重要的概率期望的公式

【19】快速傅里叶变换FFT/分治NTT/快速子集变换FWT/FST/快速莫比乌斯变换FMT

【20】康拓展开与其逆

【21】几何：射影几何中的反演定律

【22】几何：几个重要的平面几何定理

【23】代数：几个重要的不等式

【24】几何：快速凸包问题

【25】几何：半平面交

【26】几何：最近点对与最远点对

【27】几何：最小覆盖

【28】几何：费马点/皮克定理

【29】几何：非常重要的旋转卡壳与几个经典的应用

【30】几何：计算几何中的分治思想（论文）

【31】数论：连分数

【32】几何：$simpson$积分法

【33】$Kummer$定理

- $Legendre's \space formula$
  - $\nu_{p}(n !)=\sum_{i=1}^{\infty}\left\lfloor\frac{n}{p^{i}}\right\rfloor=\frac{n-s_{p}(n)}{p-1}$
  - 其中$\nu_{p}(x)$表示$x$在$p$进制下末尾$0$个数
- $Multinomial \space coefficient \space  generalization \space for \space  Kummer$
  - $\nu_{p}\left(\left(\begin{array}{c}{n} \\ {m_{1}, \ldots, m_{k}}\end{array}\right)\right)=\frac{1}{p-1}\left(\sum_{i=1}^{k} S_{p}\left(m_{i}\right)-S_{p}(n)\right)$
  - 其中$S_p(x)$表示$x$在$p$进制下的数位之和

1.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3842

【34】数论：小数与循环节

【35】数论：素数分布，素数测试

【36】数论：勾股方程与佩尔方程

【37】数论：哥德巴赫猜想、华林问题、拉格朗日四平方和定理

【38】数论：大数因数分解$Pollard_rho$算法

【39】几何：三角形的$5$心

【40】几何：四点共圆问题

【41】数论：积性函数前缀和与杜教筛

【42】组合：五边形数定理与划分数

【43】组合：基尔霍夫矩阵生成树计数

【44】组合：$Ramsey$定理

【45】组合：约瑟夫环结论

【46】组合：$prufer$编码

【47】线代：线性基

【48】数论：扩展$lucas$定理

【49】数论：完全剩余系与简化剩余系

【50】组合：置换群与波利亚计数法

【51】线代：行列式与矩阵求逆/矩阵的秩/线性相关

【52】线代：矩阵的特征值与特征向量

【53】线代：矩阵的相似对角化

【54】线代：二次型

注：一个多元二次函数，可以通过一个线性变换化为标准型，即只含变量的平方项，这样有利于求函数最值等

【55】线代：基变换与坐标变换

【56】概率论/随机过程：$Markov Chain$ 马尔可夫链与状态转移概率矩阵

【57】几何：数形结合

【58】代数：$(min,+)$卷积/最值反演/$min-max$容斥


$$
\max(S)=\sum_{T \subseteq S}(-1)^{|T|+1}\min(T)
$$

$$
\min(S)=\sum_{T \subseteq S}(-1)^{|T|+1}\max(T)
$$

$$
kth\max(S)=\sum_{T \subseteq S} (-1)^{|T|-k} {|T|-1 \choose k-1} \min(T)
$$

主要用于一些求期望的题目，求一些随机变量的最大值可以转化为求这些随机变量最小值实现

kthmax容斥这个系数是可以关于k进行递推的，如洛谷4707




$$
lcm(S)=\prod_{T\subset S}gcd(T)^{(-1)^{|T|+1}}
$$
若有
$$
g(n)=\prod _{T\subset 2^{[n]}}f(gcd_{i\in T}(i))^{(-1)^{|T|+1}}
$$
可构造出h满足
$$
f(n)=\prod _{d|n}h(d)
$$
于是
$$
g(n)=\prod _{d=1}^{n}h(d)
$$


  1.http://acm.hdu.edu.cn/showproblem.php?pid=4336

  ​	发现集合中的元素即使不是独立的好像也可以使用

  2.https://www.lydsy.com/JudgeOnline/problem.php?id=4036

  ​	min-max容斥并取反后发现要求子集和，可以用高维前缀和或者fwt

  3.https://www.luogu.org/problemnew/show/P4707

  ​	应用kthmax转换后发现就是对于容斥集合计数dp的套路，但是这样复杂度还是不够，因为k比较小，发现这个公式的系数其实是可以关于k递推的，于是就优化了复杂度，可以做了

  4.http://acm.hdu.edu.cn/showproblem.php?pid=4624

  ​	min-max容斥后转为dp求相同区间数的集合方案数，这题要高精度，比较坑

  5.https://www.lydsy.com/JudgeOnline/problem.php?id=4833

     这题套路很多，首先看出递推式后要发现有两项gcd等于下标gcd那一项的性质，然后是min-max容斥在整数上使用就是lcm-gcd容斥，然后还要构造一个h函数使
$$
  f(n) = \prod_{d|n} h(d)
$$
  改为计算每个h的贡献，发现指数被消成1了，就只要计算出h即可

  6.https://loj.ac/problem/2542

  ​	计算树上随机游走经过给定集合所有点期望次数，min-max容斥后要求第一次经过一个集合的点期望次数，虽然可以高斯消元，但复杂度不行，如果结构是树的话其实可以求每个点期望还要走多少次，然后把f[i]表示成只和f[fa[i]]以及常数b[i]有关,就可以O(n)实现了




【59】几何：$Szemerédi–Trotter \space theorem$

定理内容：

It asserts that given n points and m lines in the Euclidean plane, the number of incidences (i.e., the number of point-line pairs, such that the point lies on the line) is


$$
O(n^{2/3}*m^{2/3}+n+m)
$$

https://en.wikipedia.org/wiki/Szemer%C3%A9di%E2%80%93Trotter_theorem

使用到的题目：http://codeforces.com/problemset/problem/949/F





【60】几何：三维叉积的应用

求过两点的直线方程一般形式，判断两直线关系，并且求交点坐标

代码短，精度高，不容易出错

参考：https://blog.csdn.net/abcjennifer/article/details/7584628

摘要如下：

$$
一般方程法：\\

直线的一般方程为F(x) = ax + by + c = 0。既然我们已经知道直线的两个点，\\

假设为(x_0,y_0), (x_1, y_1)，那么可以得到a = y_0 – y_1, b = x_1 – x_0, c = x_0y_1 – x_1y_0。\\

因此我们可以将两条直线分别表示为\\

F_0(x) = a_0x + b_0y + c_0 = 0, F_1(x) = a_1x + b_1y + c_1 = 0\\

那么两条直线的交点应该满足\\

a_0x + b_0y +c_0 = a_1x + b_1y + c_1\\

由此可推出\\

x = (b_0c_1 – b_1c_0)/D\\

y = (a_1c_0 – a_0c_1)/D\\

D = a_0b_1 – a_1b_0， (D为0时，表示两直线平行)\\
$$


【61】几何：理解向量除法的定义，公式和理论解释与性质

参考资料：

http://blog.sina.com.cn/s/blog_6b7148a80102w4rg.html

https://www.zhihu.com/question/29160144




摘要如下：



**同时已知点乘和叉乘定义矢量除法运算**

若  

$$
\left\{
\begin{aligned}
\vec{a}\cdot \vec{b}=c\\
\vec{a}\times \vec{b}=\vec{d}
\end{aligned}
\right.
$$

,则有
$$
\vec{a}\times (\vec{a}\times \vec{b})=\vec{a}(\vec{a}\cdot \vec{b})-\vec{b}(\vec{a}\cdot \vec{a})
$$

解出
$$
\vec{b}=\frac{\vec{a}(\vec{a}\cdot  \vec{b})-\vec{a}\times (\vec{a}\times \vec{b})}{\vec{a}\cdot \vec{a}}=\frac{\vec{a}c-\vec{a}\times \vec{d}}{\vec{a}\cdot \vec{a}} .
$$

四、复数解释

当矢量为平面矢量时，其可与一复数对应。即

$$
\left\{
\begin{aligned}
\vec{a}&=a_{x}\vec{i}+a_{y}\vec{j}\leftrightarrow a=a_{x}+ia_{y} \\
\vec{b}&=b_{x}\vec{i}+b_{y}\vec{j}\leftrightarrow b=b_{x}+ib_{y} 
\end{aligned}
\right.
$$

则有

$$
\bar{a}b=(\vec{a}\cdot \vec{b})+i(\vec{a}\times  \vec{b})
$$

显然有

$$
b=\frac{a(\vec{a}\cdot \vec{b})+ia(\vec{a}\times \vec{b})}{\left| a \right|^{2} } (a\ne 0)
$$

注意到其点积和叉积是福函数中的一对实部和虚部，若为一般解析函数即满足Cauchy条件。



**相关性质和理解：**

A：a和b的商的模等于$a$和$b$模的商

B：a和b的商所得向量的倾斜角等于$a$的倾斜角减去$b$的倾斜角。

C：可以这样理解二维向量所蕴含的变换：

将某个二维向量所代表的平面点与原点连线的倾斜角加上一个幅角（逆时针），
然后按照一定比例放大（乘法是乘模），
除法是上述运算的逆

D：从二元运算的角度，可以得到更进一步的理解：

假设$a,b,c$均为二维点或者二维的向量，令$p=a/b,q=a-b$

可以这样理解除法和减法运算，他们表示的均为两个操作数的有序关系

也就是说，他们本身就存储了某些变换关系的具体参数，

可以具体的揭示出，利用某种或者某些变换，如何把第二个几何对象（右侧的）变换为第一个对象

所以：令方向向右的单位向量$x=(1,0)$，原点为$t=(0,0)$

则：$a/b=p/x,a-b=q-t$

他们都表示两个对象同时发生同种变换（参数相同），相对关系不变，
均转换为某种单位对象和某个具体对象的关系，这个具体对象就是运算的结果；

除法蕴含旋转和伸缩，减法蕴含平移；

这个时候，如果用运算结果“右逆运算”某个向量：$c*p,c+p$
就表示将这种关系，作用于新的对象

因此：乘法和加法是将一个关系作用于某一对象，
而除法和减法是为了得到两个对象的具体关系（或者已知关系的具体参数）

事实上，平面上任两个等模的有向线段，均可以先通过旋转缩放，然后平移得到彼此
这样的变换是唯一的，参数的获取可以参见以下模板：

	P r=(a[2]-a[1])/(b[2]-b[1]);
	P c=a[1]-b[1]*r;

注意：这里的旋转是指的是以原点为中心的旋转，如果旋转中心不是原点，可以先全体平移

上面代码中：$r$是旋转伸缩向量,$r=|r|*(cost,sint)$,表示逆时针旋转$t$，然后伸缩$|r|$比例

这样就得到了$b$线段是如何旋转伸缩到与$a$线段有向平行的线段的

$(b[1],b[2]) ---r---> (b[1],b[2])*r  ==  (b[1]*r,b[2]*r)$

然后再看看$(b[1]*r)$是如何平移得到$a[1]$的，根据前面的理解就是代码中的$c$向量

事实上，$(r,c)$已经是完备的关系表述了

因此：$y=x*r+c$，我们可以很轻松的把$x$点，通过相同的关系变换到目标点$y$




**简要模板：**

	P operator *(const P &a)const{
		return (P){x*a.x-y*a.y,x*a.y+y*a.x};
	}
	
	P operator /(const P &a)const{
		return (P){x*a.x+y*a.y,-x*a.y+y*a.x}/a.len()/a.len();
	}





【62】数论：洲阁筛

【63】数论：分治fft求两类斯特林数

【64】数论：斯特林反演

【65】代数：拉格朗日插值法/拉格朗日多项式/拉格朗日条件极值

【66】组合：一个经典的组合问题转化结论

对于前$n$个正整数构成的集合，求所有$k$元子集元素乘积之和（$1..n$中$kk$乘积之和）

答案：$ans=S[n+1][n-k+1]$,$S$表示第一类斯特林数

【67】数论：$Min\_25$筛

参考资料：https://blog.csdn.net/oi_Konnyaku/article/details/81346998

【68】代数：多项式理论

基础：$FFT$，多项式求逆/求导/求倒，$+-*/$，乘方，开方，整除，取模，求$ln$，求$exp$，生成函数，牛顿迭代，泰勒展开，任意模数$FFT$等多项式基础，积分，多项式嵌套，多点求值和插值

参考资料：https://blog.csdn.net/oi_Konnyaku/article/details/79682528

题目：

1.https://www.nowcoder.com/acm/contest/157/F

注：生成函数优化背包$dp$

题解：https://www.nowcoder.com/discuss/93531?type=101&order=3&pos=14&page=1



【69】贪心博弈：极大极小定理

【70】代数：拟阵

【71】代数：BEST定理

https://en.wikipedia.org/wiki/BEST_theorem


【72】代数：排列与笛卡尔树的关系

【73】代数：表达式树/表达式计算

【74】代数：求$n!$模大质数($fft/ntt$应用)

https://www.cnblogs.com/zzqsblog/p/8408691.html

【75】代数：拉格朗日反演公式

【76】代数：初等对称轮换多项式简单应用

https://www.cnblogs.com/zzqsblog/p/7265111.html

【77】代数：线性递推$Berlekamp-Massey(BM)$算法

https://www.cnblogs.com/zzqsblog/p/6877339.html

【78】数论：$O(1)$查询$gcd$

https://www.cnblogs.com/zzqsblog/p/5436775.html

【79】代数：$abel$阿贝尔求和变换公式

【80】组合：$gcd$卷积与$lcm$卷积

卷积是一种比较耗费计算资源的基础数学运算，在数学上我们处理卷积的一般方法都是通过各种变换或者转化，使得问题转化为比较容易计算的计算类型(比如序列点积)，想方设法加速计算的效率，当然这需要卷积本身具有一定的数学性质。

***gcd*卷积**是说我们需要计算的卷积公式为：


$$
\Large
c_k=\sum_{(i,j)=k}a_i*b_j
$$



令$A,B,C$分别为$a,b,c$的类点值序列(闭区间$[1,n]$,下标超过$n$值为$0$)，

其中一个定义如下：


$$
\Large
A_k=\sum_{k|d}a_d
$$

那么即有：

$$
\Large
C_k=\sum_{k|d}c_d=\sum_{k|d}\sum_{(i,j)=d}a_i*b_j=\sum_{k|(i,j)}a_i*b_j \\

\Large
=\sum_{k|i}\sum_{k|j}a_i*b_j=(\sum_{k|i}a_i)*(\sum_{k|i}b_i)=A_k*B_k
$$

我们得到：

$$
\Large
C=A\bullet B
$$

序列反演公式： 

$$
\Large
a_k=\sum_{k|d}A_d*\mu_{\frac{d}{k}}
$$

***lcm*卷积**是说我们需要计算的卷积公式为：


$$
\Large
c_k=\sum_{[i,j]=k}a_i*b_j
$$

令$A,B,C$分别为$a,b,c$的类点值序列，其中一个定义如下：


$$
\Large
A_k=\sum_{d|k}a_d \Leftrightarrow A=a \circ I
$$

那么即有：


$$
\Large
C_k=\sum_{d|k}c_d=\sum_{d|k}\sum_{[i,j]=d}a_i*b_j=\sum_{[i,j]|k}a_i*b_j \\

\Large
=\sum_{i|k}\sum_{j|k}a_i*b_j=(\sum_{i|k}a_i)*(\sum_{i|k}b_i)=A_k*B_k
$$

我们得到：


$$
\Large
C=A\bullet B
$$

序列反演公式： 

$$
\Large
a_k=\sum_{d|k}A_d*\mu_{\frac{k}{d}}=\sum_{x*y=k}A_x*\mu_y \Leftrightarrow a=A \circ\mu
$$

更多信息可以参见模板和配套的$md$说明文件

【81】集合幂级数和快速莫比乌斯变换$FMT$/分治乘法

参见2015国家集训队论文

【82】组合：单位根反演

【83】组合：循环卷积

简单的说，与普通FFT算法的唯一区别在于：

**变换采用的单位根的阶是与变换序列长度一样的**，因此当我们限制FFT变换的长度的时候，

会产生越界，而越界在低阶单位根中会产生循环，而卷积的本质并没有发生变化，都是选用合适的线性变换矩阵，左乘带变换的向量，进行正变换

【84】组合/数论：分圆多项式
https://yhx-12243.github.io/OI-transit/memos/17.html#pr-1-1

**Cyclotomic polynomial**

https://en.wikipedia.org/wiki/Cyclotomic_polynomial

注：参见onenote笔记



【85】组合：k进制fwt/高维广义快速离散傅里叶变换fft

**本质**：有穷高维循环卷积$fft$，循环周期为$k$

http://www.cnblogs.com/TinyWong/p/10351109.html

https://www.cnblogs.com/reverymoon/p/10197711.html

需要变换的下标每个数都是$n$位的$k$进制数，那么下标空间为$[0,k^n)$

这相当于一种$n$维的($n=log_kN$)每维长度为$n$的$fft$循环异或卷积变换($k$进制不进位加法)，按照高维$fft$的思路，应该按照某种维度的排列顺序(比如从高位到低位)，逐维正变换，然后每个位置独立做点积，最后再逐维逆变换(对应一种递归或者迭代过程)

$2$进制宏观上正变换的实质：$\large c_i=\sum_{j=0}^{2^k-1}(-1)^{num(j\&k)}a_j,i\in[0,2^k-1]$

$k$进制微观上每维正变换的实质，与$fft$相似，是**向量左乘一个变换矩阵**$T$，满足$T(i,j)*T(i,k)=T(i,j \oplus k)$

我们采用$k$阶单位根的***范德蒙德矩阵***：
$$
T=\begin{bmatrix}
 1& 1 &  1& ... & 1\\ 
 1& w_k^1&  w_k^2& ... & w_k^{k - 1}\\ 
 1&  w_k^2 &  w_k^4&  ... & w_k^{2(k - 1)}\\ 
 ...&  ...&  ...&  ...& ...\\ 
 1&  w_k^{k - 1}& w_k^{2(k - 1)} & ... & w_k^{(k - 1)(k - 1)}
\end{bmatrix}
$$
其行列式为：
$$
det(T)=\prod \limits_{i < j} (x_i - x_j)，x_i\ne x_j \\
det(T)\ne 0 \leftrightarrow T可逆
$$
其逆矩阵为：
$$
T^{-1}=\frac{1}{k} \begin{bmatrix}
 1& 1 &  1& ... & 1\\ 
 1& w_k^{-1}&  w_k^{-2}& ... & w_k^{-(k - 1)}\\ 
 1&  w_k^{-2} &  w_k^{-4}&  ... & w_k^{-2(k - 1)}\\ 
 ...&  ...&  ...&  ...& ...\\ 
 1&  w_k^{-(k - 1)}& w_k^{-2(k - 1)} & ... & w_k^{-(k - 1)(k - 1)}
\end{bmatrix}
$$
证明用到结论：
$$
[n | t] = \sum \limits_{i = 0}^{n - 1} w_n^{ti}
$$
注：2进制下的特殊情形
$$
T=\begin{bmatrix} 1& 1\\  1& -1 \end{bmatrix} =  \begin{bmatrix} 
0.5& 0.5\\
0.5& -0.5\\
\end{bmatrix}^{-1}
$$
一种**实现思路**是：

采用递归，传入参数FWT(a,S,n,op)，表示的是将a数组中以S开头的长度为n的一段区间进行正/逆变换(op=1为正/op=-1为逆)，那么首先将这段区间平均分为k段，每段长度n/k，逐段递归FWT，然后回溯合并时扫描段长(穷举一个段中偏移为i的位置)，将这些位置取出来构成一个k维向量，将这个向量左乘单位根矩阵$T$或者$T^{-1}$，变换后按顺序放置回去，对每个偏移量i都这样操作即可



**数的表示技巧：单位根表示法**

注意到一个数$x$，需要与$k$阶单位根做乘积，正常的思路是用一个$pair<double,double>$保存其复数的实部和虚部，用复数的乘法规则运算，但是这样显然精度损失严重，最终不容易回到其整数形态

注意到数$x$一定具有形式：$x=\sum_{i=0}^{k-1}a_i\omega^i$，故可以使用$k$维向量$\overrightarrow{a}$表示数$x$

那么普通的加减就是模意义下逐位加减，普通的乘法变为$k$维向量的**循环卷积**即可

而与$\omega^t$相乘相等于，此向量循环右移$t$位

考虑最后如何由向量$\overrightarrow{a}$得到整数值$x$:
$$
令cnt=k\&-k，L=k/cnt \\
容易发现，[0,k)这些下标可以分成cnt组，每组L个元素，分组的依据是一个下标i\&cnt的值的不同 \\
比如k=20可以分为以下4组： \\
$$

| 组/元素 | /4=0 | /4=1 | /4=2 | /4=3 | /4=4 |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 组0   | 0    | 4    | 8    | 12   | 16   |
| 组1   | 1    | 5    | 9    | 13   | 17   |
| 组2   | 2    | 6    | 10   | 14   | 18   |
| 组3   | 3    | 7    | 11   | 15   | 19   |

当$k$为偶数时，$0$和$k/2$这两个位置保存整数值；当$k$为奇数时，只有$0$这个唯一的位置保存整数值

我们每组独立考虑，首先$0$和$k/2$不会分到同一组，因为$k/2$存在，则必定$k$为偶数，$k$为偶数，则可以先按照每个下标的最后一位是$0$或者$1$暂时分成两组，若$0$和$k/2$同分在组$A$，则$x$轴上方和下方显然有一样多的元素属于组A，那么组$A$显然包含了偶数个元素，则组$A$，还可以继续拆分为两组，重复应用这个过程，由无穷递降法知矛盾

**基本事实**：每组单位根之和为$0$，这是因为：
$$
x^n-1=\prod_{i=0}^{n-1}(x-\omega^i)=(x-1)(x^{n-1}+x^{n-2}+\dots+1) \\
约去x-1得到：\\
x^{n-1}+x^{n-2}+\dots+1=\prod_{i=1}^{n-1}(x-\omega^i) \\
而\sum_{i=0}^{L-1}\omega_{k}^{cnt*i+t}=\omega^t(\sum_{i=0}^{L-1}\omega_{cnt*L}^{cnt*i})=\omega^t(\sum_{i=0}^{L-1}\omega_{L}^{i})=0
$$
若一个组不含$0$和$k/2$，那么这个组元素都相同，可消去为$0$；若含有其中一个，则其余元素全相同，可消除为除$0$下标之外元素为$0$；那么我们最多考虑两个组贡献，就是$a[t]-a[t+cnt],t \in \{0,k/2\}$

可以得到模板代码求整数值如下：

```c++
inline ll Value() {
	int cnt=K&-K,L=K/cnt; ll ret=a[0]-(L>1)*a[cnt];
	if (K&1^1) ret-=a[K>>1]-(L>1)*a[(K>>1)+cnt],ret%=_p;
	return ret;
}
```



**单位根表示法的优化**：

很显然，对于一个偶数进制k(k为奇数的两倍)，除了用k阶单位根表示一个数，还可以用k/2阶单位根，这主要是因为有类似于折半引理的复数性质，可以节约一些常数；如果这里可以找到一些更本质的性质，也许可以推广下去，或者针对具体的进制，具体的分析




**求逆技巧**：

注意在$FWT$的逆变换中，最中间的赋值语句要除以一个进制数，或者最终结果每个元素要除以一个长度$N=k^p$

而$FWT$正变换中没有除法，所以最终结果每个元素只要除以$N^t$，其中$t$为逆变换的总次数



**模数变更**：

当模数不是一个质数的时候，考虑进制数$k$可能和模数不互质，那么将$k$分解为$k=k'*q$，其中$q$使用数学技巧转化掉(事实上要视情况而定，可能不能转化掉)，而$k'$是互质成分，存在逆元

当存在特殊模数的时候，比如$2^{58}$，可以不取模，常数可能会小很多



**公共性质：**

卷积定理表明：
$$
T(a\oplus b)=T(a)\cdot T(b) \\
T(a+b)=T(a)+T(b) \\
T(h(a,b))=h(T(a),T(b)) \\
T(h(\overrightarrow{a}))=h(\overrightarrow{T}(\overrightarrow{a})) \\
其中h(a,b,c)是关于多项式a,b,c之间的组合多项式函数
$$




【86】组合/数论：fft应用：优化进制转化

【87】代数/数论：狄利克雷定理(用于等差数列)

**Dirichlet's theorem on arithmetic progressions**

https://en.wikipedia.org/wiki/Dirichlet%27s_theorem_on_arithmetic_progressions

【88】数论：高斯整数

**Gaussian integer**

https://en.wikipedia.org/wiki/Gaussian_integer

【89】组合：二维fft

***形式化的理解***：
$$
\Large D F T : : f(x, y)=\sum_{u=0}^{M-1} \sum_{v=0}^{N-1} F(u, v) e^{2 \pi i\left(\frac{ux}{M}+\frac{vy}{N}\right)} \\
\Large I D F T : : F(x, y)=\frac{1}{N M} \sum_{u=0}^{M-1} \sum_{v=0}^{N-1} f(u, v) e^{-2 \pi i\left(\frac{x u}{M}+\frac{y v}{N}\right)}
$$
范德蒙德矩阵：
$$
V=\left[ \begin{array}{ccccc}{1} & {x_{1}} & {x_{1}^{2}} & {\dots} & {x_{1}^{n-1}} \\ {1} & {x_{2}} & {x_{2}^{2}} & {\cdots} & {x_{2}^{n-1}} \\ {1} & {x_{3}} & {x_{3}^{2}} & {\dots} & {x_{3}^{n-1}} \\ {\vdots} & {\vdots} & {\vdots} & {\ddots} & {\vdots} \\ {1} & {x_{n}} & {x_{n}^{2}} & {\dots} & {x_{n}^{n-1}}\end{array}\right]
$$
$n$阶单位根对应的范式矩阵：令上式中的$x_i=\omega_n^i$，则$n$阶单位根一个对应一行，我们令为行向量$\overrightarrow{a_i}$

则此范式矩阵可重写为：
$$
V(n)=\left[ \begin{array}{ccccc}{\overrightarrow{\omega_n^0}} \\ {\overrightarrow{\omega_n^1}} \\ {\overrightarrow{\omega_n^2}} \\ {\vdots} \\ {\overrightarrow{\omega_n^{n-1}}} \end{array}\right]
$$
假设待变换的一维向量为$\overrightarrow{x}$：

**一维fft​**：

其正变换实质为：
$$
T(\overrightarrow{x})=V(n)*\overrightarrow{x}=\left[ \begin{array}{ccccc}{\overrightarrow{\omega_n^0} \cdot\overrightarrow{x}} \\ {\overrightarrow{\omega_n^1} \cdot \overrightarrow{x}} \\ {\overrightarrow{\omega_n^2}\cdot \overrightarrow{x}} \\ {\vdots} \\ {\overrightarrow{\omega_n^{n-1}}\cdot \overrightarrow{x}} \end{array}\right] \\
其中*表示broadcasting乘法，\cdot表示向量或者矩阵点积(内积)
$$
假设待变换的二维矩阵为$X$：

**二维fft：**

其正变换实质为：
$$
V(n,m)=V(n)*V(m)^T=\left[ \overrightarrow{\omega_n^{i}} \circ \overrightarrow{\omega_m^j }\right]_{n\times m} \\
其中*表示矩阵乘法，\circ表示向量或者矩阵卷积 \\
T(X)=V(n,m)*X=\left[\left( \overrightarrow{\omega_n^{i}} \circ \overrightarrow{\omega_m^j }\right) \cdot X \right]_{n\times m} \\
其中*表示broadcasting乘法，\cdot表示向量或者矩阵点积(内积) \\
$$
***形象化的理解***：

将所有的维度编号，且按照一定顺序排成一排，从左往右逐维度正变换(每次变换的是一个一维向量)；

两个带卷积矩阵或者张量都这样做，然后将整个超立方体或者类似结构，整体做点积(对应相乘但是不加)；

最后结果按照原来的相反顺序，逐维度做逆变换

比如$A \circ B$：先把$A$和$B$分别逐行变换，再逐列变换，形成$A'$和$B'$，然后两者做不加点积$C'=A'\cdot B'$，然后对$C'$先做逐列逆变换，再做逐行逆变换，形成$C$

**注意**：这里的$n$和$m$，是待卷积序列或者矩阵规模，不需要扩充到具体$2$的幂次，后者是具体的快速算法的实现



【90】数论：Kummer's theorem

https://en.wikipedia.org/wiki/Kummer%27s_theorem



【91】代数：暴力多项式取模$m^2logn$，用于特征多项式法解$k$阶常系数线性齐次递推数列(k>=1000)

蕴含着：Cayley–Hamilton theorem

https://en.wikipedia.org/wiki/Cayley%E2%80%93Hamilton_theorem

参考资料：

https://blog.csdn.net/joker_69/article/details/80869814

https://blog.csdn.net/hzj1054689699/article/details/85683342

有模板题和模板：***LinearRecursion***ZP版本$O(m^2logn)$

https://www.lydsy.com/JudgeOnline/problem.php?id=4161

**简要笔记**：

$O(m^2logn)$可以使用长除法，模拟多项式除法/取模(被除$deg=n \le 1e18$,除数$deg=m \le 1000$)，参见模板

令递推变换矩阵为$A_{m \times m}$，其特征多项式$G(\lambda)$为：
$$
G(\lambda)=|\lambda I-A|=\lambda^{m}-\sum_{i=0}^{m-1} a_{m-i} \lambda^{i}=[-a_m,-a_{m-1},-a_{m-2},\dots,-a_1,1]
$$
根据$Cayley–Hamilton$定理，有：$G(A)=0$

若$x^n=F(x)G(x)+C(x),deg(C)<m$，则有$A^n=C(A)$

更进一步地：$A^n \overrightarrow{x}=C(A)\overrightarrow{x}=(\sum_{i=0}^{m-1}c_iA^{i})\overrightarrow{x}=\sum_{i=0}^{m-1}c_i(A^{i}\overrightarrow{x})$

假设我们取具体而特定的：$\overrightarrow{x}^T=[x_{m-1},x_{m-2},x_{m-3},\dots,x_1,x_0]$

为了得到$x_n$，我们应该左乘$A^{n-m+1}$,取结果向量第一个元素$x_n=(A^{n-m+1}\overrightarrow{x})[1]$

我们得到：
$$
x_n=\sum_{i=0}^{m-1}c_ix_{m-1+i}
$$
上述差卷积需要已知：$X'=[x_{m-1},x_{m},x_{m+1},\dots,x_{2m-3},x_{2m-2}]=[x_i],i \in [m-1,2m-2]$

此种方法可能还需要我们多算$O(m)$项，如果我们左乘$A^{n}$取结果向量第m个元素(最后一个)，亦即：
$$
x_n=(A^n\overrightarrow{x})[m]=\sum_{i=0}^{m-1}c_i(A^{i}\overrightarrow{x})[m]=\sum_{i=0}^{m-1}c_i((A^{i}\overrightarrow{x})[m])=\sum_{i=0}^{m-1}c_ix_i=\overrightarrow{C}\cdot\overrightarrow{X} \\

其中：\overrightarrow{C}=[c_i],\overrightarrow{X}=[x_i], i \in [0,m-1],另\cdot表示向量点积
$$
可以看到，这种方法没有什么冗余计算，$\overrightarrow{C}$和$\overrightarrow{X}$均为已知的，只要直接做一次点积即可

而$\overrightarrow{C}$通过多项式$x^n$对$G(x)$取模得到，由于$n$巨大，所以不能用普通的多项式取模模板，考虑使用快速幂$Pow(x,n,G)$,令多项式$x^t$在模$G$意义下不断自乘即可，故我们需要写一个模板函数，$mul(A,B,G)$表示模$G$意义下多项式$A$和$B$乘积，其中如果多项式乘和取模用暴力$O(m^2)$，则此方法复杂度$O(m^2logn)$，而如果使用多项式模板($ntt$实现)，则复杂度为$O(mlogmlogn)$

如果我们只知道$\overrightarrow{a}=[a_i],i \in [1,m]$，和$x_0$，而不知道整个$\overrightarrow{X}$，现在要求$x_n$，就需要先求$\overrightarrow{X}$：

$O(m^2)$可以暴力线性递推，$O(mlog^2m)$可以使用分治$fft/ntt$，$O(mlogm)$可以使用以下生成函数方法：
$$
令\overrightarrow{H}=\sum_{i=0}^{+\infin}x_iz^i为普通型生成函数 \\

\overrightarrow{H}=\frac{\overrightarrow{H}(1-\overrightarrow{a})}{1-\overrightarrow{a}} \\
故：\overrightarrow{X}=\overrightarrow{H}\%x^m=\frac{\overrightarrow{H}(1-\overrightarrow{a}) \% x^m}{1-\overrightarrow{a}}=\frac{(\overrightarrow{H}\%x^m(1-\overrightarrow{a}) \% x^m)\%x^m}{(1-\overrightarrow{a})\%x^m} \\
注：上式分子实际上是个有穷多项式，特别当心\overrightarrow{a}下标是从1开始的，即[1,m]
$$

当然，上述方法适用于知道$x_0$，比较快速地求出$f[1..n],k \le n \le 10^6$

更本质地讲，如果我们把所有序列下标为负的部分，都看作$0$，那么其实$x_0$不再是序列$x$的首项

这样讲的意义在于，我们可以重构序列$\overrightarrow{X'}=[x_i],i \in [-(m-1),0]$

从而重构：$\overrightarrow{x'}^T=[x_{0},x_{-1},x_{-2},\dots,x_{-(m-2)},x_{-(m-1)}]$

我们仍然左乘$A^{n}$取结果向量第1个元素，亦即：
$$
x_n=(A^n\overrightarrow{x'})[1]=\sum_{i=0}^{m-1}c_i(A^{i}\overrightarrow{x'})[1]=\sum_{i=0}^{m-1}c_i((A^{i}\overrightarrow{x'})[1])=\sum_{i=0}^{m-1}c_ix_i=\overrightarrow{C}\cdot\overrightarrow{X} \\

其中：\overrightarrow{C}=[c_i],\overrightarrow{X}=[x_i], i \in [0,m-1],另\cdot表示向量点积
$$

发现最终需要的还是$\overrightarrow{X}$，而不是$\overrightarrow{X'}$；我们左乘$A^{n+m-1}$取结果向量第$m$个元素，亦即：

$$
x_n=(A^{n+m-1}\overrightarrow{x'})[m]=\sum_{i=0}^{m-1}c_i'(A^{i}\overrightarrow{x'})[m]=\sum_{i=0}^{m-1}c_i'((A^{i}\overrightarrow{x'})[m])=\sum_{i=0}^{m-1}c_i'x_{i-m+1}=\overrightarrow{C'}\cdot\overrightarrow{X'}=c'_{m-1}x_0 \\

其中：\overrightarrow{C'}=[c_i'],i \in [0,m-1],\overrightarrow{X'}=[x_i], i \in [-(m-1),0],另\cdot表示向量点积
$$
因此可以看到，我们不再需要计算多余的前$m$项内容，只要计算多项式快速幂模，亦即$\overrightarrow{C'}$即可

**推广：**

求递推序列$\{x_i\}$的前$n+1$项和$s_n$，沿用上述的方法：

令$C_i$表示多项式$x^i$对特征多项式$G$取模，令$C=\sum_{i=0}^nC_i=(\sum_{i=0}^nx^i)\%G$，类似于快速幂的递归算法可以求解$C$，结果仍然是$\overrightarrow{C}\cdot\overrightarrow{X}$





【92】在线性递推中，涉及到的多项式取模，倍增快速幂，以及求逆计算的fft常数优化技巧

参考资料：https://blog.csdn.net/joker_69/article/details/80869814



【93】概率论：全期望公式
$$
E(E(X|Y))=E(X) \\
注意：E(X|Y)是个随机变量，概率分布：以P(Y=y)概率取到E(X|Y=y)
$$
进一步分析可见维基百科或者2013年国家集训队论文《概率论应用》



【94】组合：超平面切平面的规律

经典问题：$n$个$k-1$维超平面最多可以将$k$维空间分割成多少个空间区域
$$
f(n,k)=\sum_{i=0}^{min(k,n)}\binom{n}{i}
$$

| $f(n,k)$ | 0    | 1    | 2    | 3    | 4    | 5    | 6    | 7    | 8    | $\dots$ |
| -------- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ------- |
| 0        | 1    | 1    | 1    | 1    | 1    | 1    | 1    | 1    | 1    | $\dots$ |
| 1        | 1    | 2    | 2    | 2    | 2    | 2    | 2    | 2    | 2    | $\dots$ |
| 2        | 1    | 3    | 4    | 4    | 4    | 4    | 4    | 4    | 4    | $\dots$ |
| 3        | 1    | 4    | 7    | 8    | 8    | 8    | 8    | 8    | 8    | $\dots$ |
| 4        | 1    | 5    | 11   | 15   | 16   | 16   | 16   | 16   | 16   | $\dots$ |

递推公式：
$$
f(0,k)=1,k \ge 0 \\
f(n,k)=f(n-1,k-1)+f(n-1,k)
$$
显然将上表中，每一行都差分一下，记得到组合数表；可以这样理解，每个第$0$行的$1$都为下面区域带来一个组合数的贡献，那么$(n,k)$相当于得到了行总是$n$但是列$\in [0,k]$的组合数贡献之和

该序列可以通过莫队算法或者分治$fft$快速求得一组，线性时间可预处理一行或者一列

特别的，令$k=2$有：直线分割平面的区域数目：
$$
f(n,2)=\binom{n}{0}+\binom{n}{1}+\binom{n}{0}=n(n+1)/2+1
$$
一些其他问题，比如折线划分平面，或者闭曲线椭圆划分平面，这些都可以用类似的类比递推归纳的方法，得到递推式，但暂时不便于推广到高维情形



【95】代数/拓扑：全序关系、偏序关系与偏序集

全序关系$\le$满足：完全性，即$\forall x,y \in S,x \le y || y \le x$

偏序关系$\le$满足：自反性(反身性)，即$\forall x \in S,x \le x$

两者均满足：

反对称性，即$\forall x,y \in S,x\le y \&\& y \le x \leftrightarrow x=y$

传递性，即$\forall x,y,z\in S, x \le y \&\& y \le z \to x \le z$

由于完全性是反身性的特例，故全序关系是偏序关系的特例，即全序关系一定是偏序关系

二者直观的区别在于，偏序关系并不是两两可比(默认只知道自己和自己可比)，但是全序关系是两两可比的



全序集及其笛卡尔积偏序线性空间中的$min/max$函数的基本性质与推广

- 都满足交换律，结合律等基本性质
- 满足对称分配率，即$min$对$max$满足分配率，反之亦然

设全序集$(S,\le)$中运算$+$表示二元$min$函数，运算$*$表示二元$max$函数，该表示可以用多元多项式刻画复杂的$min/max$嵌套表达式

令$T_n=S^n,n\in[1,+\infin]$，注意$(T_n,\le)$一般不再是全序集，但是如果定义$T_n$上的$min$为各维$min$的笛卡尔积，可以发现仍然满足上述的分配率；当$S=\{0,1\}$时，$\&$为$S^n$上的$min$，$|$为$S^n$上的$max$；当$S=N$时，$gcd$为$S^n$上的$min$，$lcm$为其$max$，可以推广到$S=Z$，涉及到有理数的$gcd$；当$S^k$为全集$U$($|U|=n$)的$k$元子集簇时，$\cap$为其$min$，$\cup$为其$max$

与$gcd$有关的分配率的直接推论：

- $lcm(gcd(x,y),gcd(x,z),gcd(y,z))=gcd(lcm(x,y),lcm(x,z),lcm(y,z))$
- $n$元整数集$(k-k)gcd$的$lcm$等于$((n-k+1)-(n-k+1))lcm$的$gcd$



【96】代数：偏序闭包



【97】代数：偏序矩阵及其行列式



【98】组合：网格图不交路径计数



【99】代数：线性基的持久化与简单扩充



【100】数论/密码学：RSA公钥体系

公钥加密，私钥解密，$RSA$可靠性取决于大数因式分解的困难性

取两个大而不太接近的质数$p,q$，令$n=pq,t=\phi(n)=(p-1)(q-1)$

取一个随机数$e \in [2,t),gcd(e,t)=1$，令$d=e^{-1}\pmod{t}$

$(n,e)$为公钥，$(p,q,d)$为私钥，明文为$M$，密文为$C$

加密算法：$C=M^e \pmod{n}$

解密算法：$M=C^d \pmod{n}$



【101】数论/密码学：$ElGamal$密码

其可靠性取决于大数离散对数的困难程度

选择一个大质数$p$，且要求$p-1$含大质因子，选择一个$p$的生成元或原根$a$

随机选择一个$d \in [2,p-2]$，令$y=a^d \pmod{p}$

公开$p,a$，取$y$为公钥，$d$为私钥，明文为$M$，密文为$(C_1,C_2)$

加密算法：随机选取$k \in [2,p-2]$

$C_1=a^k \pmod{p}$

$C_2=My^k \pmod{p}$

解密算法：$M=C_2C_1^{-d} \pmod{p}$



【102】数论/密码学：椭圆曲线密码学



【103】微积分：椭圆积分



【104】代数/拓扑：闭包/基的基本性质和运算



【105】几何：高维叉积的定义和几何性质



【106】数论：$Vantieghems theorem$

$n$是质数当且仅当：
$$
\prod_{1 \leq k \leq n-1}\left(2^{k}-1\right)\equiv n\pmod{2^n-1}
$$
可以换成其他的公式：
$$
\prod_{1 \leq k \leq n-1}\left(X^{k}-1\right) \equiv n-\left(X^{n}-1\right) /(X-1)\pmod{X^n-1} \\

\prod_{1 \leq k \leq n-1}\left(X^{k}-1\right) \equiv n \pmod{\frac{X^{n}-1}{X-1}}
$$

【107】概率论：正规数

[维基百科](https://en.wikipedia.org/wiki/Normal_number)



【108】数论：高度合成数

[维基百科](https://en.wikipedia.org/wiki/Highly_composite_number)



【109】代数：一些基本代数函数的基本性质

二进制含$1$个数奇偶性函数$p(x)$基本性质

- $p(x\oplus y)=p(x)\oplus p(y)$，即$p$对异或$\oplus$满足分配率
















##【题目：数论】

1.http://www.lydsy.com/JudgeOnline/problem.php?id=1041

2.http://www.lydsy.com/JudgeOnline/problem.php?id=1406

3.http://www.lydsy.com/JudgeOnline/problem.php?id=1951

4.http://www.lydsy.com/JudgeOnline/problem.php?id=3501

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3884

6.http://www.lydsy.com/JudgeOnline/problem.php?id=2976

7.http://www.lydsy.com/JudgeOnline/problem.php?id=1876

8.http://www.lydsy.com/JudgeOnline/problem.php?id=1876

9.http://www.lydsy.com/JudgeOnline/problem.php?id=4373

10.http://www.lydsy.com/JudgeOnline/problem.php?id=4454

11.http://www.lydsy.com/JudgeOnline/problem.php?id=4488

12.http://www.lydsy.com/JudgeOnline/problem.php?id=4522

13.http://www.lydsy.com/JudgeOnline/problem.php?id=2721

14.http://www.lydsy.com/JudgeOnline/problem.php?id=2186

15.http://www.lydsy.com/JudgeOnline/problem.php?id=4544

16.http://www.lydsy.com/JudgeOnline/problem.php?id=2401

17.http://www.lydsy.com/JudgeOnline/problem.php?id=3601

18.http://www.lydsy.com/JudgeOnline/problem.php?id=2219

注：离散对数解高次同余方程模板，本题要求模数取奇数，详细分析过程参见网上题解或者上面知识点笔记

19.http://www.lydsy.com/JudgeOnline/problem.php?id=4176

20.http://www.lydsy.com/JudgeOnline/problem.php?id=4772

21.http://www.lydsy.com/JudgeOnline/problem.php?id=2277

22.http://www.lydsy.com/JudgeOnline/problem.php?id=1968

23.http://www.lydsy.com/JudgeOnline/problem.php?id=4635

24.http://www.lydsy.com/JudgeOnline/problem.php?id=4173

25.http://www.lydsy.com/JudgeOnline/problem.php?id=2818

//阅读一些积性函数求和的资料
http://blog.csdn.net/skywalkert/article/details/50500009

26.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1244

27.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1239

28.http://acm.hdu.edu.cn/showproblem.php?pid=5608

29.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1584

30.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1220

31.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1222

32.http://www.spoj.com/problems/DIVCNT2/

33.http://tsinsen.com/A1231

34.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1227

35.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1237

36.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1238

37.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1847

38.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1575

39.http://www.spoj.com/problems/DIVCNT3/

40.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemId=5340

41.http://www.lydsy.com/JudgeOnline/problem.php?id=3512

42.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3881

43.http://www.lydsy.com/JudgeOnline/problem.php?id=2693

44.http://www.lydsy.com/JudgeOnline/problem.php?id=2749

45.http://www.lydsy.com/JudgeOnline/problem.php?id=3930

46.http://www.lydsy.com/JudgeOnline/problem.php?id=2142

47.http://www.lydsy.com/JudgeOnline/problem.php?id=2629

注：$lucas$定理+$fft$+离散对数+高精度+分类讨论

一道不难且不错的题目，给定：质数$p=51061$，$n<p^{k}$，$k=10$

求组合数第$n$行关于模数$p$的分布，即给出$cnt[i]$表示余数恰好为$i$的元素个数

由于$n$为大整数且$p$不大，故联想到$lucas$定理，将$n$拆为$p$进制数$n_tn_{t-1}\cdots n_0$

则有：$\binom{n_t}{k_t}\binom{n_{t-1}}{k_{t-1}}\cdots \binom{n_0}{k_0}=i\pmod{p}$

由于$\binom{n_j}{k_j}=\frac{n_j!}{k_j!(n_j-k_j)!}$，故显然可以$O(p)$复杂度求其关于模$p$的分布(假设有$q$个$p$进制为，预处理复杂度显然为$O(q*p)$)

揉入上式，即得到一个狄利克雷循环卷积，利用离散对数转化为，普通循环和卷积，之后$fft$

注意答案中$0$这种情况可以特殊考虑，因为$0$元素没有离散对数，与$lucas$结合也很容易变为数位$dp$

事实上，只要简单容斥一下，即用总数$n+1$减去其余情况数量之和即可；而余数不为$0$的和也等于$\prod_{i=0}^t(n_i+1)$

另外注意，本题虽然结果模$29$，但是$10$重卷积，$fft$不特殊处理可能仍然溢出

48.http://www.lydsy.com/JudgeOnline/problem.php?id=3992

注：比较基础的离散对数，化狄利克雷循环卷积为普通循环卷积，基础的生成函数用到多项式循环乘方，由于空间开不下，还是牺牲一个$log$复杂度用快速幂好，注意每次循环叠加清空

49.http://www.lydsy.com/JudgeOnline/problem.php?id=4128

注：经典的矩阵同余方程，一般情况是不大容易解的，数据保证$p$以内有解；利用$BSGS$的分块思想，随机向量判矩阵相等$A=B\times C$的$hash$思想

50.http://www.lydsy.com/JudgeOnline/problem.php?id=2480

51.http://www.lydsy.com/JudgeOnline/problem.php?id=1420

52.http://www.lydsy.com/JudgeOnline/problem.php?id=3527

53.http://www.lydsy.com/JudgeOnline/problem.php?id=2194

54.http://www.lydsy.com/JudgeOnline/problem.php?id=2179

55.http://www.lydsy.com/JudgeOnline/problem.php?id=3456

56.http://www.lydsy.com/JudgeOnline/problem.php?id=3557

57.http://www.lydsy.com/JudgeOnline/problem.php?id=3160

58.http://www.lydsy.com/JudgeOnline/problem.php?id=3771

59.http://www.lydsy.com/JudgeOnline/problem.php?id=4555

60.http://acm.hdu.edu.cn/showproblem.php?pid=5322

61.http://acm.hdu.edu.cn/showproblem.php?pid=5896

62.http://acm.hdu.edu.cn/showproblem.php?pid=5730

63.http://acm.hdu.edu.cn/showproblem.php?pid=3634

64.http://acm.hdu.edu.cn/showproblem.php?pid=5279

65.http://acm.hdu.edu.cn/showproblem.php?pid=5126

66.http://acm.hdu.edu.cn/showproblem.php?pid=1402

67.http://acm.hdu.edu.cn/showproblem.php?pid=5197

68.http://acm.hdu.edu.cn/showproblem.php?pid=5751

69.http://acm.hdu.edu.cn/showproblem.php?pid=3864

70.http://acm.hdu.edu.cn/showproblem.php?pid=3939

71.http://acm.hdu.edu.cn/showproblem.php?pid=6211

72.http://acm.hdu.edu.cn/showproblem.php?pid=2815

73.http://acm.hdu.edu.cn/showproblem.php?pid=1320

74.http://acm.hdu.edu.cn/showproblem.php?pid=2522

75.http://acm.hdu.edu.cn/showproblem.php?pid=2814

76.http://acm.hdu.edu.cn/showproblem.php?pid=6034

77.http://www.lydsy.com/JudgeOnline/problem.php?id=3301

78.http://www.lydsy.com/JudgeOnline/problem.php?id=3143

79.http://www.lydsy.com/JudgeOnline/problem.php?id=3118

80.http://www.lydsy.com/JudgeOnline/problem.php?id=4269

81.http://www.lydsy.com/JudgeOnline/problem.php?id=2844

82.http://www.lydsy.com/JudgeOnline/problem.php?id=1778

83.http://www.lydsy.com/JudgeOnline/problem.php?id=1770

84.http://www.lydsy.com/JudgeOnline/problem.php?id=3817

85.http://poj.org/problem?id=2987

86.http://www.lydsy.com/JudgeOnline/problem.php?id=2705

87.http://www.lydsy.com/JudgeOnline/problem.php?id=2694

88.http://www.lydsy.com/JudgeOnline/problem.php?id=4820

89.http://www.lydsy.com/JudgeOnline/problem.php?id=1101

90.http://poj.org/problem?id=2154

91.http://www.lydsy.com/JudgeOnline/problem.php?id=1407

92.http://www.lydsy.com/JudgeOnline/problem.php?id=3782

93.http://www.lydsy.com/JudgeOnline/problem.php?id=1951

94.http://acm.hdu.edu.cn/showproblem.php?pid=1573

95.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1028

96.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1348

97.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1514

98.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1387

99.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1172

100.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1258

101.http://www.lydsy.com/JudgeOnline/problem.php?id=3684

102.http://www.lydsy.com/JudgeOnline/problem.php?id=4735

103.http://www.lydsy.com/JudgeOnline/problem.php?id=4911

104.http://www.lydsy.com/JudgeOnline/problem.php?id=4504

105.http://www.lydsy.com/JudgeOnline/problem.php?id=4589

106.http://codeforces.com/problemset/problem/449/D

107.http://codeforces.com/contest/663/problem/E

108.http://acm.hdu.edu.cn/showproblem.php?pid=5823

109.http://acm.hdu.edu.cn/showproblem.php?pid=6057

110.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1773

111.http://acm.hdu.edu.cn/showproblem.php?pid=5909

112.http://www.spoj.com/problems/VECTAR1/

113.http://www.spoj.com/problems/TSUM/en/

114.http://www.spoj.com/problems/VFMUL/

115.http://www.ifrog.cc/acm/problem/1028

116.http://codeforces.com/gym/101480    //F题

117.http://poj.org/problem?id=2389

118.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3899

119.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3874

120.http://codeforces.com/problemset/problem/901/E

121.http://codeforces.com/problemset/problem/906/D

122.http://codeforces.com/problemset/problem/919/E

123.http://codeforces.com/problemset/problem/920/G

124.http://acm.hdu.edu.cn/showproblem.php?pid=6298

125.https://nanti.jisuanke.com/t/30999

126.https://nanti.jisuanke.com/t/31444

127.https://nanti.jisuanke.com/t/31448

128.https://nanti.jisuanke.com/t/31456

129.http://www.51nod.com/onlineJudge/questionCode.html#!problemId=1965

130.https://loj.ac/problem/6053

131.https://www.spoj.com/problems/DIVCNTK/

132.http://codeforces.com/problemset/problem/1031/F

133.https://www.lydsy.com/JudgeOnline/problem.php?id=5348

134.https://www.lydsy.com/JudgeOnline/problem.php?id=3122

注：经典问题，问一个值在一个线性同余递推数列中的最小出现下标，分类讨论，指数同余，离散对数

135.https://www.lydsy.com/JudgeOnline/problem.php?id=3285

注：基础题，拆开换元后，变成指数同余方程，离散对数

136.http://acm.hdu.edu.cn/showproblem.php?pid=6051

注：离散对数+数论函数求和

题意：令$f(i)$表示方程$(x+y)^i=x^i\pmod{p}$，$p$为质数且$x \in [1,p-1],y \in [1,m]$，给定$m,p$求$\sum_{i=1}^{p-1}if(i)$
$$
两边同取离散对数，得到：\\
ilog_g(x+y)=ilog_gx\pmod{p-1}\\
亦即：log_g(x+y)=log_gx\pmod{\frac{p-1}{gcd(i,p-1)}}\\
故有：log_g(1+\frac{y}{x})=0\pmod{\frac{p-1}{gcd(i,p-1)}}\\
注意：这里的\frac{1}{x}是模p意义下的，不是模那个约数意义下的，指标才是\\
分析1+\frac{y}{x}\ge 2的离散对数的可能取值，[1,p-2]且为那个约数模数的倍数，注意不能取0\\
故1+\frac{y}{x}，亦即\frac{y}{x}有gcd(i,p-1)-1种合法取值，而x\in[1,p-1]相当于循环群全集\\
而y\in[1,m]，限制更强，枚举并固定y，有gcd(i,p-1)-1种不同且合法的x与之对应\\
故：f(i)=m(gcd(i,p-1)-1)
$$
最后的求和是不值一提的，非本题的难点

137.http://acm.hdu.edu.cn/showproblem.php?pid=5478

注：2015上海区域赛真题，不认为是什么好题，可以直接用暴力完美代替离散对数，简单分析如下：

简单说，就是给一个方程对$n\in Z_+$恒成立，由于取$n$为奇数有比较好的性质，故公式可化为：
$$
(k_1n+b)log_ga-(k_2(n-1)+1)log_g(-b)=0\pmod{c-1}\\
令n=1，又可得到：\\
(k_1+b)log_ga-log_g(-b)=0\pmod{c-1}\\
立即解出x，令p=k_1k_2+bk_2-k_1：\\
p(n-1)x=0\pmod{c-1}，n为奇数\\
即：\\
nx=0\pmod{\frac{c-1}{2gcd(p,c-1)}记作p'}，n\in[0,+\infin)，分母的2如果不能整除就不除\\
显然这等价于：x=0\pmod{p'}，也就是只需要check\space O(gcd)级别的x(即a的指标)即可
$$

138.http://acm.hdu.edu.cn/showproblem.php?pid=5377zhu

注：批量$BSGS$，不能直接求离散对数，由于有多个模数，固定之，求以其原根为底的一大组数的离散对数

化为解线性同余方程，注意特殊情况的处理

139.http://acm.hdu.edu.cn/showproblem.php?pid=4861

注：简单的初等数论分析题，令$f(i)=\sum_{x=0}^{p-1}x^i\pmod{p}$，令集合$S=\{f(i),i\in[1,k]\}$，给定$p,k$($p$为质数)，求集合$S$分布；看起来这是等幂和模序列的形式，有经典的公式，但是最好是从原根的角度分析该问题：

令$g$为模$p$原根，因为$[1,p-1]$为模$p$的完系或循环群，故每个元素有唯一的指标，故：$f(i)=\sum_{t=0}^{p-2}(g^i)^t$，若$g^i=1\pmod{p}$为等差数列，即$f(i)=p-1$，$\phi(p)=p-1|i$，这样的$i$在$[1,k]$中显然有$\lfloor\frac{k}{p-1}\rfloor$；否则，由欧拉定理，$f(i)=\frac{1-g^{i(p-1)}}{1-g^i}=0$.

注意：以上公式在一些特殊情况下，如$i=p$，是有更直接的性质的，但是要千万小心小的特例，如$p=2,g=1$情况；这正如在经典的威尔逊定理中，小心$n=4$的情况是不成立的

140.http://acm.hdu.edu.cn/showproblem.php?pid=2619

注：求原根数量，一般的结论中注意原根存在才有$phi(phi(m))$个原根








##【题目：组合】

1.http://www.lydsy.com/JudgeOnline/problem.php?id=1008

2.http://www.lydsy.com/JudgeOnline/problem.php?id=1089

3.http://www.lydsy.com/JudgeOnline/problem.php?id=1227

4.http://www.lydsy.com/JudgeOnline/problem.php?id=2012

5.http://www.lydsy.com/JudgeOnline/problem.php?id=2111

6.http://www.lydsy.com/JudgeOnline/problem.php?id=2729

7.http://www.lydsy.com/JudgeOnline/problem.php?id=3198

8.http://www.lydsy.com/JudgeOnline/problem.php?id=3505

9.http://www.lydsy.com/JudgeOnline/problem.php?id=3622

10.http://www.lydsy.com/JudgeOnline/problem.php?id=4086

11.http://www.lydsy.com/JudgeOnline/problem.php?id=4305

12.http://www.lydsy.com/JudgeOnline/problem.php?id=4403

13.http://www.lydsy.com/JudgeOnline/problem.php?id=1101

14.http://www.lydsy.com/JudgeOnline/problem.php?id=2005

15.http://www.lydsy.com/JudgeOnline/problem.php?id=2154

16.http://www.lydsy.com/JudgeOnline/problem.php?id=2190

17.http://www.lydsy.com/JudgeOnline/problem.php?id=2301

18.http://www.lydsy.com/JudgeOnline/problem.php?id=2671

19.http://www.lydsy.com/JudgeOnline/problem.php?id=2705

20.http://www.lydsy.com/JudgeOnline/problem.php?id=3309

21.http://www.lydsy.com/JudgeOnline/problem.php?id=3529

22.http://www.lydsy.com/JudgeOnline/problem.php?id=3834

23.http://www.lydsy.com/JudgeOnline/problem.php?id=3994

24.http://www.lydsy.com/JudgeOnline/problem.php?id=3944

25.http://www.lydsy.com/JudgeOnline/problem.php?id=1025

26.http://www.lydsy.com/JudgeOnline/problem.php?id=1902

27.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3638

28.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3233

29.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3556

30.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3868

31.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2836

32.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3435

33.http://acm.hdu.edu.cn/showproblem.php?pid=1085

34.http://acm.hdu.edu.cn/showproblem.php?pid=1171

35.http://acm.hdu.edu.cn/showproblem.php?pid=1398

36.http://acm.hdu.edu.cn/showproblem.php?pid=2079

37.http://acm.hdu.edu.cn/showproblem.php?pid=2082

38.http://acm.hdu.edu.cn/showproblem.php?pid=2110

39.http://acm.hdu.edu.cn/showproblem.php?pid=2152

40.http://acm.hdu.edu.cn/showproblem.php?pid=2189

41.http://acm.hdu.edu.cn/showproblem.php?pid=2566

42.http://www.lydsy.com/JudgeOnline/problem.php?id=1488

43.http://www.lydsy.com/JudgeOnline/problem.php?id=1004

44.http://acm.hdu.edu.cn/showproblem.php?pid=2865

45.http://poj.org/problem?id=2888

46.http://acm.hdu.edu.cn/showproblem.php?pid=3923

47.https://uva.onlinejudge.org/index.php?option=com_onlinejudge&Itemid=8&page=show_problem&problem=1542

48.http://codeforces.com/problemset/problem/914/G

49.http://codeforces.com/problemset/problem/932/E

50.http://codeforces.com/problemset/problem/938/E

51.http://codeforces.com/problemset/problem/955/C

52.http://acm.hdu.edu.cn/showproblem.php?pid=5245

53.http://acm.hdu.edu.cn/showproblem.php?pid=6390

54.http://codeforces.com/problemset/problem/958/F3

[经典]求x1+x2+...xk==n的有上下界的不定方程整数解组数

注：分治fft/启发式合并fft

55.https://www.codechef.com/problems/CUTTREE

56.https://nanti.jisuanke.com/t/31453

57.https://nanti.jisuanke.com/t/31713

58.https://www.lydsy.com/JudgeOnline/problem.php?id=3625

[经典]类卡特兰数列递推，生成函数，多项式开根和求逆

59.https://codeforces.com/problemset/problem/852/F

60.http://codeforces.com/problemset/problem/1045/H

61.https://vjudge.net/contest/274676#problem/J

62.https://vjudge.net/contest/274500#problem/L

63.http://codeforces.com/gym/101955/problem/C

64.http://codeforces.com/gym/101955/problem/M

65.http://codeforces.com/gym/102012/problem/G

66.http://codeforces.com/gym/101981/attachments J题

67.http://codeforces.com/problemset/problem/1091/D

68.http://codeforces.com/problemset/problem/1096/E

69.http://codeforces.com/problemset/problem/1096/G

70.http://codeforces.com/problemset/problem/1097/D

71.http://codeforces.com/problemset/problem/1097/F

注：gcd卷积，二进制(模2)意义下bitset优化，容斥或者莫比乌斯函数反演变换，一些简单的预处理技巧；关于gcd卷积的简单介绍，参见上面的知识点讲解

72.http://codeforces.com/problemset/problem/1097/G

注：树形dp，树上合并式背包，斯特林变换公式，k次幂组合意义，容斥原理

斯特林公式：
$$
n^k=\sum_{i=1}^kS(k,i)*i!*C(n,i)
$$
注意：此公式是转化形如n^k元素的有用途径，当然可以很方便的在公式表中找到

73.http://codeforces.com/problemset/problem/1010/F

注：经典题目，树上多项式合并：树上差分+基础组合+树链剖分+重链上分治+fft/ntt

二叉树，树上每个叶子多项式为x+1，每个中间节点多项式等于儿子多项式乘积*x+1；

重链剖分，重链上每个节点缓存其轻儿子贡献和(*x)，再对重链分治：重链上每个节点等于重儿子+1之后乘自己的多项式，求重链根的多项式，相当于简单的分治法，求以下表达式的值：

$$
a_1(a_2(a_3(a_4+1)+1)+1)=a_1a_2a_3a_4+a_1a_2a_3+a_1a_2+a_1\\

=a_1a_2(a_3a_4+a_3)+a_1a_2+a_1
$$

直接按照项数将表达式一分为二，左边简单提取之后，发现很容易维护二元组(各数乘积f，表达式值g)的合并：

$$
\left\{
\begin{aligned}
f=f_lf_r \\
g=f_lg_r+g_l
\end{aligned}
\right.
$$

时间复杂度是n(logn)^3，树剖、分治、fft各占一个log


74.https://www.lydsy.com/JudgeOnline/problem.php?id=5093

75.http://codeforces.com/problemset/problem/286/E

注：思维题+背包+闭包/线性空间+fft

76.http://codeforces.com/problemset/problem/662/C

注：比较隐蔽的异或卷积模型，已知隐蔽的函数f(x)=x的二进制表示中0和1的个数最小值

求
$$
min \sum_if(a_i \oplus x), x \in [0,2^n)\\

denote: A_i=f(i),B_i=count(i),or that:B_{a_i}++\\

fwt:A \oplus B
$$

77.http://codeforces.com/problemset/problem/632/E

注：简单生成函数+多项式乘方，注意只需要知道最终结果每个系数是否为0，ntt双模数hash思想

78.http://codeforces.com/problemset/problem/827/E

注：求带?的01串的所有可能周期，等价于对周期t，任意i有：a[i]与a[i-kt]不矛盾，fft/ntt可用差卷积求a[i]与a[i-t]的矛盾性，数组ret[t]并上所有t倍数的矛盾性，即ret[kt]即可


79.http://codeforces.com/problemset/problem/715/E

注：考察卷积的组合意义，fft/ntt+容斥/二项式反演+第一类斯特林数


80.http://codeforces.com/problemset/problem/755/G

注：特征根法解行生成函数的递推方程+多项式基本操作(求逆，乘方，开方等)

做法1：

$$
f[i][j]=f[i-1][j]+f[i-1][j-1]+f[i-2][j-1] \\

那么 f[n] 作为行生成函数满足： \\

\begin{array}{l}{f_{n}(x)=f_{n-1}(x)+x f_{n-1}(x)+x f_{n-2}(x)} \\ {=(x+1) f_{n-1}(x)+x f_{n-2}(x)}\end{array}\\

f_{i}=C_{1} * T 1(x)^{i}+C_{2} * T_{2}(x)^{i}\\

T1和T2为以下特征根方程的两根：\\

T^{2}(x) - (x+1)T(x) - x = 0\\

\triangle=x^2+6x+1\\

T_{1}(x)=\frac{1+x+\sqrt\triangle}{2}\\

T_{2}(x)=\frac{1+x-\sqrt\triangle}{2}\\

已知:\\

f_0=C_1+C_2=1\\

f_1=C_1*T_1+C_2*T_2=1+x\\

故：\\

C_1=\frac{T_2-(1+x)}{T_2-T_1}\\

C_2=\frac{T_1-(1+x)}{T_1-T_2}\\

注意到，由韦达定理：\\

T_1+T_2=-\frac{b}{a}=1+x\\

T_2-T_1=\sqrt\triangle\\

故：\\

C_1=\frac{T_1}{\sqrt\triangle}\\

C_2=-\frac{T_2}{\sqrt\triangle}\\

则：\\

\large f_n=\frac{T_1^{n+1}-T_2^{n+1}}{\sqrt\triangle}\\

由于：T_2常数项为0，故T_2^{n+1}最低次超过n\\

故：只需计算f_n=\frac{T_1^{n+1}}{\sqrt\triangle}\\
$$

做法2：多项式倍增



81.http://codeforces.com/problemset/problem/1119/H

注：取值稀疏的特殊情况下，多重异或卷积的fwt优化

fwt原理/性质+特殊值法构造方程组

题目：若干个数组求其多重异或卷积，每个数组由一个三元组(a,b,c)构造，表示T[a]=x,T[b]=y,T[c]=z,(x,y,z)对所有数组相同且题目给定

关键点1：一步转化，如果直接对某个数组T做fwt变换后，所有下标均被填上值，且值的种类最多8种

而如果我们对元祖(a,b,c)进行变换(0,b\^a,c\^a)，此步操作相等于对数组做一个异或卷积，卷积数组为P(P[a]=1,其余为0)，最终将结果还原回来即可（数组下标变换异或X=所有a的异或和）

此步转化，将fwt后的值的种类减少为最多4种

这4种值固定为：

$$
v_1=x+y+z\\

v_2=x+y-z\\

v_3=x-y+z\\

v_4=x-y-z\\
$$

关键点2：考虑fwt的如下性质：

$$
fwt(A+B)=fwt(A)+fwt(B)\\

fwt(A \circ B)=fwt(A)*fwt(B)\\

考虑将所有数组fwt之后相乘，下标j的结果p中包含A_j个v_1，B_j个v_2，C_j个v_3，D_j个v_4\\

故：A_j*v_1+B_j*v_2+C_j*v_3+D_j*v_4=p\\

即：\\

A_j*(x+y+z)+B_j*(x+y-z))+C_j*(x-y+z)+D_j*(x-y-z)=p\\

整理为：\\

x*(A_j+B_j+C_j+D_j)+y*(A_j+B_j-C_j-D_j)+Z*(A_j-B_j+C_j-D_j)=p\\

注意这里是x，y，z不局限于题目读入的数据，可以带入任意的整数：\\

考虑任意三元组都可以分拆为单位向量的线性组合，故我们取单位向量带入：\\

A_j+B_j+C_j+D_j=a\\

A_j+B_j-C_j-D_j=b\\

A_j-B_j+C_j-D_j=c\\

还少一个方程，但是线性空间已经用完，需要挖掘一个新的：\\

我们考虑取：对于元祖(a,b,c)，取T[b xor c]++\\

fwt(\sum_{i=1}^{n}T_i)=fwt(\sum_{i=1}^{n}P_i\circ Q_i)\\

=\sum_{i=1}^{n}fwt(P_i\circ Q_i)=\sum_{i=1}^{n}fwt(P_i)fwt(Q_i)\\

考虑两个数组P和Q，第一个只有y=1(b xor a)，第二个只有z=1(c xor a)，二者分别fwt：\\

任意位置都是+-1，b xor c得到的数组，等于这两个的卷积，那么fwt之后，就是对应位置的乘积\\

观察v_1,v_2,v_3,v_4的构造，取x=0,发现y=1和z=1交换时，v_2和v_3会变号，v_1和v_4不变号，\\

因而新的值v和旧的值v二者相乘，中间两个数变为-1，故B_j和C_j是乘-1，其余两个乘1，故得到：\\

A_j-B_j-C_j+D_j=d\\

逐位解方程，快速幂计算ret[]之后，UFWT，再下标异或X变换回去即可\\
$$



82.http://codeforces.com/problemset/problem/528/D

注：预处理+fft/ntt，预处理每个下标每个字母是否可以放，然后每种字母独立考虑做一次差卷积

83.http://codeforces.com/problemset/problem/993/E

注：01数组，问有多少个区间使得其区间和为k，0<=k<=n，输出n+1个答案

中国剩余定理crt+fft/ntt，答案没有取模，采用两个模数ntt合并

84.https://www.lydsy.com/JudgeOnline/problem.php?id=5478

85.https://www.lydsy.com/JudgeOnline/problem.php?id=5411

86.https://www.lydsy.com/JudgeOnline/problem.php?id=5475

87.https://www.lydsy.com/JudgeOnline/problem.php?id=5330

88.https://www.lydsy.com/JudgeOnline/problem.php?id=5298

89.https://www.lydsy.com/JudgeOnline/problem.php?id=5283

90.https://www.lydsy.com/JudgeOnline/problem.php?id=5221

91.https://www.lydsy.com/JudgeOnline/problem.php?id=5217

92.http://codeforces.com/problemset/problem/754/E

注：二维单模式串匹配问题，模式串带通配符，bitset或者二维fft应用

传统的独立考虑每种字母方法，由于字符集有一定规模，外加fft/ntt常数较大，远远超时；

考虑应用于复数域序列变换的二维fft，对主串中每个元素(字母)，如果不是通配符，填充$e^{i\theta},\theta=2\pi/M*k,k\in[0,M-1]$其中M为字符集大小，k为字符编号，通配符填充复数cp{0,0}

对模式串每个字母，选用$\theta'=-\theta$即可，且统计模式串中非通配符的字符数量tot，考虑与模式串同规模的主串子矩形，与模式串对应做点积，由于通配符与任意字符直接相乘为0，对于两个非通配符字母来说，当且仅当为同种字母时，相乘才为1(否则，乘积的实部一定小于1，只要有一对不匹配，最终结果就一定严格小于tot)，比较点积结果实部是否为tot即可

另外，如果主串也带通配符，那么就应该用两次二维fft，第二次中令模式串和主串的通配符为整数0，其他字母为整数1，这样卷积可以算出每个位置为起点的理应达到的点积整数值(如果匹配成功)，取代原来的全局tot变量，然后逐位相比较即可

其他做法，一个在一维世界中流行的做法：

就是构造一对字符的匹配函数h(x,y)使得当x和y为同种字符函数值取0，其他搭配函数值取正整数值；

构造两个等长字符串(带通配符)的匹配函数H(s,t)意义同上，构造过程为以上函数的对应叠加；考虑快速计算每个位置的匹配函数值，一般反转模式串，将表达式拆开为若干部分，分别做卷积即可

93.https://www.lydsy.com/JudgeOnline/problem.php?id=4503

注：上面这题的一维弱化版本，同样的，仅模式串带通配符

94.http://codeforces.com/problemset/problem/472/G

注：分块+fft，对第一个串分块，预处理每一个块和第二个串整串的差卷积；

技巧：沿用上面这题的思想，考虑将0字符填充为-1,1字符填充为1，那么两个等长序列的匹配数x或者不匹配数y(相同字符数目或者不同字符数目)，可以通过解方程组确定：卷积得到x-y，而x+y为序列长度

思想：主要思想就是单位根，相同字符点积为1，不同为-1，其实1和-1是2次单位复数根

注意：这个题目比较卡时间，暴力压64位或者bitset可能会更快，最好使用fft_fast模板来减少fft的常数，加速其变换过程

95.http://codeforces.com/group/aUVPeyEnI2/contest/243687 G

注：抽屉原理/鸽巢原理+处理gcd



96.http://codeforces.com/problemset/problem/981/H

注：树dp+生成函数+分治fft/ntt+暴力多项式除法+简单容斥

复杂度分析用到：树上子树大小sz[]数组，最多只会有根号种不同取值

一些经典的树上计数问题，常常将路径分为两类，垂直链和非垂直链，分开计算答案，常常维护根到点的信息并

非垂直链可以用使用容斥原理，在垂直链上计算负的贡献



97.http://uoj.ac/problem/272

98.http://codeforces.com/problemset/problem/1103/E

注：k进制FWT模板题，注意模数为$2^{58}$，$long long$可以不取模；当然十进制意义下，用五阶单位根表示数，可以节约一半的时间

99.http://acm.hdu.edu.cn/showproblem.php?pid=4447

100.http://codeforces.com/problemset/problem/1054/H

注：中国剩余定理crt+离散对数与原根+二维狄利克雷循环卷积+小型容斥

狄利克雷循环卷积取离散对数转化为普通循环卷积，循环卷积扩充一倍体积转为普通卷积，二维fft

注意这里循环卷积循环周期不是一个质数，要分解为若干质数独立考虑；

而分解的实质是，对于每个下标$i$，将$i$变换为一个元祖$\overrightarrow{a}$(高维空间中的一个点)，其中$a_k$表示$i$对质数$p_k$的余数的离散对数；在高维空间对矩阵或者张量做$DFT$，计算好卷积之后，再进行压缩变换，变为一维序列；所以需要预处理一定范围内的离散对数和高维空间点与序列下标的对应映射关系

101.http://codeforces.com/problemset/problem/145/D

注：复杂的计数结构题，所谓计数结构是这样一种机制，保证可以不重复不遗漏的计数对象

枚举左边区间的右端点，步进其左端点，遇到新的未出现的关键点，去右边区间更新"不交线段并"，维护右边区间的非法数目，容斥原理

102.http://codeforces.com/problemset/problem/848/E

注：环状计数dp+生成函数/多项式求逆/分治fft

首先分类讨论表示多个dp状态，推导出简单的卷积递推式，此时可以分治fft；

表示成生成函数的方程组，解方程组，此时可以多项式求逆；

对生成函数进行进一步化简，使得其分子分母次数界不超过40，此时就可以暴力计算多项式乘除了

参考题解：*注意题解公式部分有误*

https://www.luogu.org/problemnew/solution/CF848E

核心公式如下：
$$
生成函数方程组：\\

\begin{aligned} F_{0}(z) &=G_{0}(z)+G_{0}(z) F_{0}(z) z+G_{1}(z) F_{1}(z) z^{3} \\ F_{1}(z) &=G_{1}(z)+G_{1}(z) F_{0}(z) z+G_{2}(z) F_{1}(z) z^{3} \\ F_{2}(z) &=G_{2}(z)+G_{1}(z) F_{1}(z) z+G_{2}(z) F_{2}(z) z^{3} \end{aligned}
$$

$$
解得：\\

\begin{aligned} F_{0}(z)=& \frac{G_{1}^2(z) z^{3}-G_{0}(z)\left(G_{2}(z) z^{3}-1\right)}{\left(G_{0}(z) z-1\right)\left(G_{2}(z) z^{3}-1\right)-G_{1}^{2}(z) z^{4}} \\ F_{1}(z)=& \frac{G_{1}(z)}{\left(G_{0}(z) z-1\right)\left(G_{2}(z) z^{3}-1\right)-G_{1}^{2}(z) z^{4}} \\ & F_{2}(z)=\frac{G_{2}(z)+G_{1}(z) z F_{1}(z)}{1-G_{2}(z) z^{3}} \end{aligned}
$$

$$
令：\\\begin{array}{c}{Q(z)=-z^{12}-3 z^{10}+5 z^{6}-3 z^{2}+1} \\ {P_{0}(z)=16 z^{8}+12 z^{6}+20 z^{4}+4 z^{2}} \\ {P_{1}(z)=9 z^{8}+2 z^{6}+23 z^{4}+6 z^{2}+1} \\ {P_{2}(z)=4 z^{8}-4 z^{6}+24 z^{4}+4 z^{2}+4}\end{array}
$$

$$
G可表示为：\\

G_{0,1,2}(z)=\frac{P_{0,1,2}(z)}{Q(z)}
$$

$$
代入即得：\\

\begin{aligned} F_{0}(z) &=\frac{P_{1}^2(z) z^{3}-P_{0}(z)\left(P_{2}(z) z^{3}-Q(z)\right)}{\left(P_{0}(z) z-Q(z)\right)\left(P_{2}(z) z^{3}-Q(z)\right)-P_{1}^{2}(z) z^{4}} \\ F_{1}(z) &=\frac{P_{1}(z) Q(z)}{\left(P_{0}(z) z-Q(z)\right)\left(P_{2}(z) z^{3}-Q(z)\right)-P_{1}^{2}(z) z^{4}} \end{aligned}
$$

$$
F_{1}(z)=\frac{M(z)}{N(z)}
$$

$$
F_{2}(z)=\frac{N(z) P_{2}(z)+P_{1}(z) M(z) z}{N(z)\left(Q(z)-P_{2}(z) z^{3}\right)}
$$

$$
最终答案：\\

ans=(g(n-1)+g(n-3))(n-1)^{2} + \\

\sum_{i=2}^{n-2} i(i-1)^{2}\left(g(i-1) f_{0}(n-i-1)+2 g(i-2) f_{1}(n-i-2)+g(i-3) f_{2}(n-i-3)\right)
$$

103.https://www.lydsy.com/JudgeOnline/problem.php?id=4161

注：k阶线性递推模板题，复杂度$k^2logn$









##【题目：几何】

1.http://www.lydsy.com/JudgeOnline/problem.php?id=1043

2.http://www.lydsy.com/JudgeOnline/problem.php?id=2433

3.http://www.lydsy.com/JudgeOnline/problem.php?id=3203

4.http://www.lydsy.com/JudgeOnline/problem.php?id=4427

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3533

6.http://www.lydsy.com/JudgeOnline/problem.php?id=3228

7.http://www.lydsy.com/JudgeOnline/problem.php?id=2657

8.http://www.lydsy.com/JudgeOnline/problem.php?id=2300

9.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3598

10.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3728

11.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3783

12.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=1041

13.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2287

14.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3913

15.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2675

16.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2967

17.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=1081

18.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2394

19.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=1049

20.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=1696

21.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=1648

22.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=1450

23.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=1090

24.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=2287

25.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3203

26.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3762

27.http://acm.hdu.edu.cn/showproblem.php?pid=3548

28.http://acm.hdu.edu.cn/showproblem.php?pid=5784

29.http://acm.hdu.edu.cn/showproblem.php?pid=2202

30.http://acm.hdu.edu.cn/showproblem.php?pid=2510

31.http://acm.hdu.edu.cn/showproblem.php?pid=1451

32.http://acm.hdu.edu.cn/showproblem.php?pid=2105

33.http://acm.hdu.edu.cn/showproblem.php?pid=4142

34.http://acm.hdu.edu.cn/showproblem.php?pid=2039

35.http://acm.hdu.edu.cn/showproblem.php?pid=4709

36.http://acm.hdu.edu.cn/showproblem.php?pid=5135

37.http://acm.hdu.edu.cn/showproblem.php?pid=3629

38.http://acm.hdu.edu.cn/showproblem.php?pid=4798

39.http://acm.hdu.edu.cn/showproblem.php?pid=1007

40.http://acm.hdu.edu.cn/showproblem.php?pid=4458

41.http://acm.hdu.edu.cn/showproblem.php?pid=4720

42.http://acm.hdu.edu.cn/showproblem.php?pid=2187

43.http://acm.hdu.edu.cn/showproblem.php?pid=5251

44.http://poj.org/problem?id=2187

45.http://poj.org/problem?id=2079

46.http://www.spoj.com/problems/CIRU/

47.http://acm.fzu.edu.cn/problem.php?pid=1007

48.http://acm.fzu.edu.cn/problem.php?pid=1510

49.http://acm.fzu.edu.cn/problem.php?pid=1485

50.http://acm.fzu.edu.cn/problem.php?pid=1482

51.http://acm.fzu.edu.cn/problem.php?pid=1472

52.http://acm.fzu.edu.cn/problem.php?pid=1393

53.http://acm.fzu.edu.cn/problem.php?pid=1333

54.http://acm.fzu.edu.cn/problem.php?pid=1332

55.http://acm.fzu.edu.cn/problem.php?pid=1331

56.http://acm.fzu.edu.cn/problem.php?pid=1329

57.http://acm.fzu.edu.cn/problem.php?pid=1302

58.http://acm.fzu.edu.cn/problem.php?pid=1195

59.http://acm.fzu.edu.cn/problem.php?pid=1129

60.http://acm.fzu.edu.cn/problem.php?pid=1120

61.http://acm.fzu.edu.cn/problem.php?pid=1088

62.http://acm.fzu.edu.cn/problem.php?pid=1066

63.http://acm.fzu.edu.cn/problem.php?pid=1035

64.http://acm.fzu.edu.cn/problem.php?pid=1032

65.http://acm.fzu.edu.cn/problem.php?pid=1015

66.http://acm.fzu.edu.cn/problem.php?pid=1014

67.http://www.lydsy.com/JudgeOnline/problem.php?id=1069

68.http://www.lydsy.com/JudgeOnline/problem.php?id=1185

69.http://www.lydsy.com/JudgeOnline/problem.php?id=3680

70.http://www.lydsy.com/JudgeOnline/problem.php?id=1845

71.http://www.lydsy.com/JudgeOnline/problem.php?id=2618

72.http://acm.hdu.edu.cn/showproblem.php?pid=2297

73.http://acm.hdu.edu.cn/showproblem.php?pid=5462

74.http://acm.hdu.edu.cn/showproblem.php?pid=3761

75.http://www.lydsy.com/JudgeOnline/problem.php?id=3190

76.http://www.lydsy.com/JudgeOnline/problem.php?id=1137

77.http://www.lydsy.com/JudgeOnline/problem.php?id=2732

78.https://vjudge.net/contest/187746#problem/H

79.http://www.lydsy.com/JudgeOnline/problem.php?id=4418

80.http://www.spoj.com/problems/CIRU/

81.http://www.spoj.com/problems/CIRUT/

82.http://acm.hdu.edu.cn/showproblem.php?pid=1724

83.https://uva.onlinejudge.org/index.php?option=com_onlinejudge&Itemid=8&category=446&page=show_problem&problem=4077

84.https://uva.onlinejudge.org/index.php?option=com_onlinejudge&Itemid=8&category=23&page=show_problem&problem=2119

85.http://www.lydsy.com/JudgeOnline/problem.php?id=2178

86.http://www.lydsy.com/JudgeOnline/problem.php?id=1502

87.https://vjudge.net/contest/189689#problem/D

88.https://nanti.jisuanke.com/t/30993

89.https://nanti.jisuanke.com/t/31446

90.http://codeforces.com/gym/101955/problem/L

91.http://codeforces.com/gym/102012/problem/M

92.http://codeforces.com/gym/101981/attachments D题

[注]空间最小球覆盖经典几何模型

93.https://codeforces.com/gym/101611/problem/J

注：找一个在矩形中，但不在n个三角形内或上的点；n个三角形为整点三角形且在矩形内，且面积和不超过矩形面积：二分+三角形与矩形交/差分扫描线算法

94.http://codeforces.com/group/aUVPeyEnI2/contest/243686 L题

注：经典的差分扫描线算法+利用截面积函数做定积分算体积(牛顿莱布尼兹定理)

95.http://codeforces.com/group/aUVPeyEnI2/contest/243687 K题

注：简单多边形+三角剖分，将其分成两部分面积相等，且均为简单多边形

96.https://codeforces.com/problemset/problem/70/D

注：动态凸包模板题，动态加点，动态查询给定点是否在凸包内

97.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=10433 L题

注：毒瘤的几何压轴题，求三维空间内三个半径两两不等且两两不交的球体的三维凸包体积，内含球体公切面等模板

98.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=10433 H题

注：不错的几何题，给定$k$维空间(坐标$\in [0,1e5]$)$n \le 18$个平行于坐标面的超立方体，求一个未被覆盖的字典序最小的单元超立方小格；贪心+二分+容斥+优化

字典序最小，往往逐维贪心，二分判断超立方体体积并在某一维上的坐标前缀中是否是满的(假设前面的维度被压缩到某个点值，当前维度取前缀，后面的维度取满)；由于中间结果可能巨大无比，最好用哈希思想判满；

体积并的投影，相当于体积投影的并，可以将一些二分中的可预处理的量提出去，降低复杂度

超立方体体积并是几何中经典问题，使用容斥原理







##【题目：线代】

1.http://codeforces.com/problemset/problem/845/G

2.http://codeforces.com/problemset/problem/724/G

3.http://codeforces.com/problemset/problem/938/G

4.http://codeforces.com/problemset/problem/388/D

5.http://codeforces.com/problemset/problem/895/C

6.http://codeforces.com/problemset/problem/587/E

7.http://codeforces.com/problemset/problem/504/D

8.https://www.lydsy.com/JudgeOnline/problem.php?id=2460

9.https://www.lydsy.com/JudgeOnline/problem.php?id=4184

10.https://www.lydsy.com/JudgeOnline/problem.php?id=3811

11.https://www.lydsy.com/JudgeOnline/problem.php?id=4568

12.https://www.lydsy.com/JudgeOnline/problem.php?id=4004

13.https://www.lydsy.com/JudgeOnline/problem.php?id=2115

14.https://www.lydsy.com/JudgeOnline/problem.php?id=2844

15.https://www.lydsy.com/JudgeOnline/problem.php?id=3105

16.https://www.lydsy.com/JudgeOnline/problem.php?id=4269

17.https://www.lydsy.com/JudgeOnline/problem.php?id=4671

18.https://www.lydsy.com/JudgeOnline/problem.php?id=3563

19.https://www.lydsy.com/JudgeOnline/problem.php?id=3569

20.https://www.lydsy.com/JudgeOnline/problem.php?id=3759

21.https://www.lydsy.com/JudgeOnline/problem.php?id=4644

22.https://www.lydsy.com/JudgeOnline/problem.php?id=3237

23.https://www.lydsy.com/JudgeOnline/problem.php?id=2322

24.http://acm.hdu.edu.cn/showproblem.php?pid=3949

25.http://acm.hdu.edu.cn/showproblem.php?pid=5544

26.http://codeforces.com/problemsets/acmsguru/problem/99999/275

27.https://www.51nod.com/onlineJudge/questionCode.html#!problemId=1577

28.https://www.51nod.com/onlineJudge/questionCode.html#!problemId=1323

29.http://acm.hdu.edu.cn/showproblem.php?pid=5244

30.http://codeforces.com/problemset/problem/959/F

31.http://codeforces.com/problemset/problem/958/D2

注：模意义下整数向量的线性子空间基的计算处理和hash

32.http://acm.hdu.edu.cn/showproblem.php?pid=6395

33.https://www.nowcoder.com/acm/contest/147/A

34.https://nanti.jisuanke.com/t/31000

35.https://nanti.jisuanke.com/t/31463

36.https://codeforces.com/gym/101611/problem/I

注：平方算法解异或方程组





37.https://www.lydsy.com/JudgeOnline/problem.php?id=3811

或者http://uoj.ac/problem/36

注：异或空间上的概率期望经典问题，异或空间的投影与投影空间

给定一个序列，随机选择一个子序列(可以为空)，求异或和$k$次幂的数学期望，$1 \le k \le 5$

将序列插入线性基，构造异或空间，令$m$表示空间中的最大二进制长度，令随机变量$X$表示子序列异或和
$$
\large E(X^k)=E((\sum_{i=0}^{m-1}x_i*2^i)^k)=E(\sum_{i_1=0}^{m-1}\sum_{i_2=0}^{m-1}\sum_{i_3=0}^{m-1}\dots\sum_{i_k=0}^{m-1}2^{\Large{\sum_{t=1}^ki_t}}\prod_{t=1}^{k}x_{i_t}) \\
\large =\sum_{i_1=0}^{m-1}\sum_{i_2=0}^{m-1}\sum_{i_3=0}^{m-1}\dots\sum_{i_k=0}^{m-1}2^{\Large{\sum_{t=1}^ki_t}}E(\prod_{t=1}^{k}x_{i_t}) \\
\large =\sum_{i_1=0}^{m-1}\sum_{i_2=0}^{m-1}\sum_{i_3=0}^{m-1}\dots\sum_{i_k=0}^{m-1}2^{\Large{\sum_{t=1}^ki_t}}P(\prod_{t=1}^{k}x_{i_t}=1) \\
\large 令随机变量Y=X[i_1;i_2;i_3;\dots;i_k]=(x_{i_1}x_{i_2}x_{i_3}\dots x_{i_k})_2 \\
\large 则P(\prod_{t=1}^{k}x_{i_t}=1)=P(Y=2^k-1)
$$

我们转而研究随机变量$Y$，注意到$Y$是随机变量$X$在二进制表示上的一种投影变量，令投影变换为$T$

假设选取概率空间中一个元素(实质是一个元祖)：$e=(a_1,a_2,..,a_j)$，这里只是$a$数组中任$j$个不同下标

则：异或空间对应的元素为$X(e)=a_1 \space xor \space a_2 \space xor \space \space \dots \space xor \space a_j$

$$
\large Y(e)=T(X(e))=T(xor_{i=1}^ja_i)=xor_{i=1}^jT(a_i)=X(T(e)) \\
\large 故Y是投影概率空间\{T(e)\}上的异或和随机变量
$$
**子集概率空间和异或空间的关系性质**

假设$n$个元素的序列的子集构成概率空间，那么显然概率空间中有$2^n$个元素，那么作用于这些元素的异或和随机变量$X$的分布构成另一个空间称之为异或空间，假设异或空间具有$m$个线性异或无关的异或基向量(将这$n$个元素插入到线性基结构中得到$size$为$m$的一组基)，那么异或空间有$2^m$个元素，每种对应概率空间的$2^{n-m}$个元素

证明：这$n$个元素中，一定可以找到一组$size$为$m$的线性基，剩下的$n-m$个元素，称为非基元素，事实上很容易用一一对应理论证明，非基元素的子集与异或和为$y$的方案一一对应；取上述任一子集，若子集中元素异或和为$x$，则在基元素集合中，一定可以找到$x \space xor \space  y$的唯一分解或者表示，并之即得一唯一确定方案；取任一方案，其在非基元素集合上的投影显然是唯一确定的

寻找给定异或空间元素$y$的一组在原序列上的拆分表示，即是寻找一个概率空间的元素$e$与之对应，确定一组基之后，$y$可以唯一的表示为基的线性组合，$y$具有唯一的坐标，是一个长度为$m$的二进制串

**本题思路**

我们可以先求出原序列的投影序列，然后插入到线性基结构中构造投影异或空间，但是当投影变换本身是一个枚举量且序列$a$中元素较多时，时间成本太高；其实我们可以先求出原序列的一组线性基，然后只要对基向量进行投影即可，注意到投影变换本质上是一种降维变换，所以投影过后的基向量组可能是有维度信息冗余的，所以再将新的基向量插入到线性基结构，即可构造出新的线性基及其异或空间

令新的线性基$size=m'$，如果元素$2^k-1$在新的异或空间出现，则必与其他元素等概率出现，故$P(Y=2^k-1)=\frac{1}{2^{m'}}$
$$
E(X^k)=\sum_{i_1=0}^{m-1}\sum_{i_2=0}^{m-1}\sum_{i_3=0}^{m-1}\dots\sum_{i_k=0}^{m-1}[2^k-1 \space \in \space V]2^{\Large{\sum_{t=1}^ki_t}-m'}，V表示新的异或空间
$$
事实上，$\sum_{t=1}^ki_t-m' \ge -1$，这表示结果乘$2$一定是整数，证明如下：

假设$i_1,i_2,i_3,\dots,i_k$中，不同的数有$p$个，那么考虑投影序列中的每个数是个$p$维向量，若干个$p$维向量的最大线性无关组元素个数最多为$p$($p$个基足以表示$p$维空间)，因此$m' \le p$，而$\sum_{t=1}^ki_t \ge 0+1+2+\dots+(p-1)=(p-1)*p/2$，故$\sum_{t=1}^ki_t-m' +1 \ge (p-1)*p/2-p+1=(p-1)(p-2)/2 \ge 0，\forall \space p \ge 1$

**总结**

在异或空间中，线性基不光可以求与给定数$x$做$xor$的最值(同或$\sim x$转异或)，还可以求与给定数$x$做$and$的最值，当然也可以求与给定数$x$做$or$的最值，这是因为：$(y \space or \space x)_{op}=(y \space and \space \sim x) _{op}\space or \space x$





38.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=10433 E题

注：经典问题：求高维空间两直线间最小距离，目前已知本题有4种做法

**做法1**：二次型，换主元思想

设直线$AB$与$CD$上各有一点$P$和$Q$，则$P:a\overrightarrow{A}+b\overrightarrow{B},a+b=1$

同理，$Q$的参数设为$c,d$；故

$$
|PQ|^2=(a\overrightarrow{A}+b\overrightarrow{B}-c\overrightarrow{C}-d\overrightarrow{D})^2\\
=a^2\overrightarrow{A}^2+b^2\overrightarrow{B}^2+c^2\overrightarrow{C}^2+d^2\overrightarrow{D}^2\\
+2ab\overrightarrow{A}\cdot\overrightarrow{B}+2cd\overrightarrow{C}\cdot\overrightarrow{D} \\
-2ac\overrightarrow{A}\cdot\overrightarrow{C}-2bd\overrightarrow{B}\cdot\overrightarrow{D} \\
-2bc\overrightarrow{B}\cdot\overrightarrow{C}-2ad\overrightarrow{A}\cdot\overrightarrow{D}\\
=x_1a^2+x_2b^2+x_3c^2+x_4d^2 \\ 
+2abx_5+2cdx_6-2acx_7-2bdx_8-2bcx_9-2adx_{10} \\
将b=1-a,d=1-c带入得：\\
=X_1a^2+X_2a+X_3c^2+X_4c+X_5ac+X_6
$$

其中：
$$
X_1=x_1+x_2-2x_5 \\
X_2=2x_5+2x_8-2x_{10}-2x_2 \\
X_3=x_3+x_4-2x_6 \\
X_4=2x_6+2x_8-2x_9-2x_4 \\
X_5=2x_9+2x_{10}-2x_7-2x_8 \\
X_6=x_2+x_4-2x_8
$$
考虑拉格朗日极值法，令其偏导为$0$得到方程组：
$$
2aX_1+X_2+X_5c=0 \\
2cX_3+X_4+X_5a=0 \\
解得：\\
a=\frac{2X_2X_3-X_4X_5}{X_5^2-4X_1X_3} \\
c=\frac{2X_1X_4-X_2X_5}{X_5^2-4X_1X_3}
$$
带入得到一般情况答案：
$$
ans=\frac{-X_2^2X_3-X_1X_4^2+X_2X_4X_5+4X_1X_3X_6-X_5^2X_6}{4X_1X_3-X_5^2}
$$
注意当原题意两直线平行时，要特判：因为$a,c$解出来分母为$0$，此种情况可以用向量点积直接求出答案



**做法2：**二次型化为标准型

需要二次型的线代模板



**做法3：**推广三维情形，寻找法向量求点积；这是一种几何与代数结合的方法，计算量较小

*三维情形：*

当两直线平行时，即$|\overrightarrow{AB}\cdot \overrightarrow{CD}|=|\overrightarrow{AB}||\overrightarrow{CD}|$，令$l=\frac{|\overrightarrow{AC}\cdot\overrightarrow{AB}}{|\overrightarrow{AB}|}|,d^2=\overrightarrow{AC}^2-l^2$

当两直线不平行时，过其中一条做平行于另一条的平面，将问题转化为求直线到与其平行(或共面)的一平面距离，令该平面法向量$\overrightarrow{n}=\overrightarrow{AB}\times\overrightarrow{CD},d=\frac{|\overrightarrow{AC}\cdot\overrightarrow{n}|}{|\overrightarrow{n}|}$

*推广：*

平行时，可以推广；不平行时，由于我们对于高维空间内两向量叉积定义不明晰，所以不利于推广

我们从三维情形，发现不平行时，最短距离满足一个几何性质：如果我们可以找到$p\in AB,q\in CD$且$pq \perp AB,pq \perp CD$，则$d=|pq|$

故代数化：令$p=a\overrightarrow{A}+b\overrightarrow{B},a+b=1$，$q=c\overrightarrow{C}+d\overrightarrow{D},c+d=1$
$$
\overrightarrow{pq}\perp\overrightarrow{AB},\overrightarrow{pq}\perp\overrightarrow{CD} \\
等价于\\
a\overrightarrow{A}\cdot\overrightarrow{AB}+b\overrightarrow{B}\cdot\overrightarrow{AB}-c\overrightarrow{C}\cdot\overrightarrow{AB}-d\overrightarrow{D}\cdot\overrightarrow{AB}=0 \\
a\overrightarrow{A}\cdot\overrightarrow{CD}+b\overrightarrow{B}\cdot\overrightarrow{CD}-c\overrightarrow{C}\cdot\overrightarrow{CD}-d\overrightarrow{D}\cdot\overrightarrow{CD}=0\\
换元并代入消元:\\
p_1a+p_2(1-a)+p_3c+p_4(1-c)=0\\
q_1a+q_2(1-a)+q_3c+q_4(1-c)=0\\
整理并换元:\\
s_1a+s_2c=s_3\\
t_1a+t_2c=t_3\\
解得:\\
a=\frac{s_2t_3-s_3t_2}{s_2t_1-s_1t_2}=\frac{r_1}{p}\\
c=\frac{s_3t_1-s_1t_3}{s_2t_1-s_1t_2}=\frac{r_2}{p}\\
代入|\overrightarrow{pq}|^2中计算答案:\\
ans=\frac{|r_1\overrightarrow{A}+(p-r_1)\overrightarrow{B}-r_2\overrightarrow{C}-(p-r_2)\overrightarrow{D}|^2}{p^2}
$$
**做法4:**

二分+$SternBrocot$树，目前尚不明晰其具体做法



**总结**

对于这种偏向量表述的几何题，有时候也是很受算法竞赛欢迎的；

最好是可以结合几何与代数的方法，几何上寻找一些明显的性质，代数上用细致的推理；

这样有利于得到精确解，如果对精度要求不高的话，可以用二分三分等逼近算法





39.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=10433  K题

注：简单的高斯消元模板题，构造方案










【题目：积分/多项式/概率期望】

1.http://acm.hdu.edu.cn/showproblem.php?pid=4808

2.http://acm.hdu.edu.cn/showproblem.php?pid=6305

3.http://acm.hdu.edu.cn/showproblem.php?pid=6410

4.http://acm.hdu.edu.cn/showproblem.php?pid=6362

5.http://cogs.pro:8080/cogs/problem/problem.php?pid=2189

6.https://loj.ac/problem/151

7.http://codeforces.com/problemset/problem/1096/F

8.http://codeforces.com/problemset/problem/1139/D

注：概率期望+容斥原理

经典的概率期望问题，维护一个多重集合$S$，开始为空，每次从$[1,m]$中随机生成一个数，插入到$S$中

该过程直到$gcd(S)=1$停止，求$E(sz(S))$

**非负整数随机变量数学期望的性质**：期望转概率和
$$
E(X)=\sum_{i \ge 1}P(X \ge i) \\
直接用定义证明： \\
E(X)=\sum_{x \ge 1}x*P(X=x)=\sum_{x \ge 1}P(X=x)\sum_{i=1}^x1=\sum_{i \ge 1} \sum_{x \ge i}P(X=x)=\sum_{i \ge 1}P(X \ge i)
$$
**莫比乌斯函数$O(nlogn)$容斥预处理**：代码短
$$
\sum_{d|n}\mu(d)=[n=1] \space \Rightarrow \space \mu(n)=-\sum_{d|n \\ d<n}\mu(d),n>1 \\
\mu(j)-=\mu(i),i|j,j>i
$$

**本题思路**
$$
令停止时sz(S)-1为随机变量X,其中1为停止所花的代价 \\
P(X \ge i)表示长度为i的gcd>1的序列概率, \\
p(i)表示一次随机生成一个i的倍数的元素概率：\\
p(i)=\lfloor\frac{m}{i}\rfloor/m \\
P(X \ge i)=-\sum_{k \ge 2}\mu(k) p(k)^i \\
E(X)=\sum_{i \ge 1}P(X \ge i)=-\sum_{i \ge 1}\sum_{k \ge 2}\mu(k)p(k)^i=-\sum_{k \ge 2}\mu(k)\sum_{i \ge 1}p(k)^i=-\sum_{k \ge 2}\mu(k)\frac{p(k)}{1-p(k)}
$$









【基础题集合】

1.http://codeforces.com/problemset/problem/929/C

2.http://codeforces.com/problemset/problem/938/C

3.http://codeforces.com/problemset/problem/954/E

4.http://codeforces.com/contest/145/problem/D

注：简单枚举+容斥+线段判交，整点线段上整点个数公式：gcd(|x1-x2|,|y1-y2|)+1






【签到级别数学题】

1.https://nanti.jisuanke.com/t/30990

2.https://nanti.jisuanke.com/t/31716

3.https://vjudge.net/contest/274500#problem/C

4.http://codeforces.com/problemset/problem/1093/D

5.http://codeforces.com/problemset/problem/1096/C

6.http://codeforces.com/problemset/problem/1152/C

注：gcd/lcm的性质+约数枚举




【基础几何】

1.http://codeforces.com/problemset/problem/958/E1

【递归数列专题】

1.http://acm.hdu.edu.cn/showproblem.php?pid=6304

【二进制按位贪心】

1.https://vjudge.net/contest/274676#problem/G

【表达式计算】

1.https://nanti.jisuanke.com/t/31443

2.https://www.lydsy.com/JudgeOnline/problem.php?id=3360

3.http://acm.hdu.edu.cn/showproblem.php?pid=1237

4.http://acm.hdu.edu.cn/showproblem.php?pid=1296

5.http://acm.hdu.edu.cn/showproblem.php?pid=4192

6.http://acm.hdu.edu.cn/showproblem.php?pid=5553

7.http://codeforces.com/group/aUVPeyEnI2/contest/243686 J题



【游戏状态设计和转移】

1.http://codeforces.com/gym/101955/problem/K

【区间背包和/多项式区间乘积】

1.http://codeforces.com/gym/101955/problem/M

【容斥原理小专题：邻接型容斥】

1.http://codeforces.com/gym/102012/problem/G

2.https://vjudge.net/contest/274676#problem/J

【群论基础】

1.http://codeforces.com/problemset/problem/1091/C

注：置换的乘方，等差数列求和

【括号序列】

1.http://codeforces.com/problemset/problem/1095/E





# 8.高级暴力

cf上的题目建议多看写别人的代码，如果我以前有做的，可以看我的：


【1】分块思想（重点）

1.http://www.lydsy.com/JudgeOnline/problem.php?id=2141

2.http://www.lydsy.com/JudgeOnline/problem.php?id=2120

3.http://www.lydsy.com/JudgeOnline/problem.php?id=3798

4.http://acm.hdu.edu.cn/showproblem.php?pid=5213

5.http://acm.hdu.edu.cn/showproblem.php?pid=3333

6.http://acm.hdu.edu.cn/showproblem.php?pid=4391

7.https://vjudge.net/problem/CodeChef-FNCS

8.http://acm.hdu.edu.cn/showproblem.php?pid=4677

9.http://acm.hdu.edu.cn/showproblem.php?pid=5840

10.http://acm.hdu.edu.cn/showproblem.php?pid=5110

11.http://acm.hdu.edu.cn/showproblem.php?pid=6035

12.http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=1654

13.http://acm.hdu.edu.cn/showproblem.php?pid=4676

14.http://codeforces.com/contest/551/problem/E

15.http://codeforces.com/contest/19/problem/E

16.http://codeforces.com/contest/103/problem/D

17.http://codeforces.com/contest/101/problem/E

18.http://www.lydsy.com/JudgeOnline/problem.php?id=3674（用分块做）

19.https://www.lydsy.com/JudgeOnline/problem.php?id=1086

20.https://nanti.jisuanke.com/t/31451

21.http://acm.hdu.edu.cn/showproblem.php?pid=4366

22.http://acm.hdu.edu.cn/showproblem.php?pid=4858

23.http://acm.hdu.edu.cn/showproblem.php?pid=5919

24.http://acm.hdu.edu.cn/showproblem.php?pid=6394

25.http://acm.hdu.edu.cn/showproblem.php?pid=5057

26.https://loj.ac/problem/6278

27.https://loj.ac/problem/6281

28.https://loj.ac/problem/6283

29.https://loj.ac/problem/6284

30.http://acm.hdu.edu.cn/showproblem.php?pid=4960

31.http://acm.hdu.edu.cn/showproblem.php?pid=1166

32.http://acm.hdu.edu.cn/showproblem.php?pid=5145

33.http://acm.hdu.edu.cn/showproblem.php?pid=4787

34.http://acm.hdu.edu.cn/showproblem.php?pid=5412

35.https://www.lydsy.com/JudgeOnline/problem.php?id=5087

36.https://www.lydsy.com/JudgeOnline/problem.php?id=3585

37.https://www.lydsy.com/JudgeOnline/problem.php?id=3343

38.https://www.lydsy.com/JudgeOnline/problem.php?id=4765

39.https://www.lydsy.com/JudgeOnline/problem.php?id=2388

40.https://www.lydsy.com/JudgeOnline/problem.php?id=4216

41.https://www.lydsy.com/JudgeOnline/problem.php?id=3236

42.https://www.lydsy.com/JudgeOnline/problem.php?id=4241

43.https://www.lydsy.com/JudgeOnline/problem.php?id=4537

44.https://www.lydsy.com/JudgeOnline/problem.php?id=5089

45.https://www.lydsy.com/JudgeOnline/problem.php?id=4867

46.https://www.lydsy.com/JudgeOnline/problem.php?id=5016

47.https://www.lydsy.com/JudgeOnline/problem.php?id=2741

48.http://codeforces.com/problemset/problem/1093/E

注：分块+二维树状数组(主要解决二维树状数组空间太大的问题)

49.http://codeforces.com/problemset/problem/13/E

注：简单分块+并查集，也可以用lct(注意模板中rev标记不能删除)








【2】莫队算法（重点）

http://hzwer.com/category/c/data-structure/basic-data-structure/piecemeal/



1.http://codeforces.com/contest/86/problem/D

2.http://codeforces.com/contest/13/problem/E

3.http://codeforces.com/contest/785/problem/E

4.http://codeforces.com/group/mbTSbPlZPV/contest/100513/problem/A

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3289

6.http://www.lydsy.com/JudgeOnline/problem.php?id=3757

7.http://www.lydsy.com/JudgeOnline/problem.php?id=2038

8.http://www.lydsy.com/JudgeOnline/problem.php?id=4358

9.http://acm.hdu.edu.cn/showproblem.php?pid=6333

10.http://acm.hdu.edu.cn/showproblem.php?pid=4638




【带修改】

1.http://www.lydsy.com/JudgeOnline/problem.php?id=2120

2.http://codeforces.com/problemset/problem/940/F

3.uva12345

4.https://www.lydsy.com/JudgeOnline/problem.php?id=1878



【树上莫队】

**子树树上莫队**

一个子树对应的是dfs序上连续的一段

**路径树上莫队**

我们假设要询问一条路径a-b，设lca为p=lca(a,b)。不妨设st[a]<=st[b]（否则交换一下）。

当p=a时，这应该是一个比较简单的情形：a-b是一段父子链。

我们考虑这个新dfs序上[st[a],st[b]]的点，我们可以发现，a-b上的点被算了一遍，其他点都被算了2遍或0遍！那么我们统计的时候注意一下就可以了。

当p≠a时，我们也要一样统计[ed[a], st[b]]/[st[b], ed[a]的点（从ed[a]开始为保证a不会被排除掉），但是这回lca不会被统计到，所以要另外算一下。

1.http://uoj.ac/problem/58

2.https://www.lydsy.com/JudgeOnline/problem.php?id=3052

3.http://acm.hdu.edu.cn/showproblem.php?pid=6291

4.https://www.lydsy.com/JudgeOnline/problem.php?id=4129

5.https://www.lydsy.com/JudgeOnline/problem.php?id=3757

6.https://www.lydsy.com/JudgeOnline/problem.php?id=3460

7.https://www.lydsy.com/JudgeOnline/problem.php?id=2589

8.https://www.lydsy.com/JudgeOnline/problem.php?id=4940

9.https://vjudge.net/contest/274676#problem/E




【3】高维前缀和（重点）

1.http://codeforces.com/contest/449/problem/D

注 ：问一堆数有多少种方案and起来是0，用容斥转化为求有结果不为0的方案数，然后这个要用高维前缀和来处理有多少数字可选。	

(非)2.http://codeforces.com/problemset/problem/799/F

注 ：求所有和给定区间是不交或交长度是奇数的区间和，应该有数据结构的做法，不过有做法是用随机数加xor搞过去，和高维前缀和没什么关系，只是有不少前缀和而已

3.https://www.lydsy.com/JudgeOnline/problem.php?id=5092

注 ：符合前缀性质的都可以这样做，可以维护前缀min，这样可以知道固定几位的那种数字最早什么时候出现。

【4】常数优化论文（了解）

【5】整体二分和cdq分治

论文：

《浅谈数据结构题的几个非经典解法》


学习：http://blog.163.com/bill125_zjh/blog/static/2318010062014124101819643/

https://www.cnblogs.com/shanxieng/p/10175731.html

https://www.cnblogs.com/HQHQ/p/5966453.html

https://blog.csdn.net/fo0Old/article/details/78284212



1.http://www.lydsy.com/JudgeOnline/problem.php?id=3262

2.http://codeforces.com/contest/678/problem/F

3.http://codeforces.com/contest/607/problem/E

4.http://www.lydsy.com/JudgeOnline/problem.php?id=2683

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3110

6.http://www.lydsy.com/JudgeOnline/problem.php?id=1492

7.http://codeforces.com/contest/396/problem/C

8.https://www.lydsy.com/JudgeOnline/problem.php?id=2001

9.https://www.lydsy.com/JudgeOnline/problem.php?id=2253

10.https://www.lydsy.com/JudgeOnline/problem.php?id=2716

11.https://www.lydsy.com/JudgeOnline/problem.php?id=1935

12.https://www.lydsy.com/JudgeOnline/problem.php?id=4700

13.https://www.lydsy.com/JudgeOnline/problem.php?id=4170

14.https://www.lydsy.com/JudgeOnline/problem.php?id=3263

15.https://www.lydsy.com/JudgeOnline/problem.php?id=2989

16.https://www.lydsy.com/JudgeOnline/problem.php?id=2773

17.https://www.lydsy.com/JudgeOnline/problem.php?id=2244

18.https://www.lydsy.com/JudgeOnline/problem.php?id=4137

19.http://codeforces.com/problemset/problem/762/E

20.http://codeforces.com/problemset/problem/938/G

21.http://codeforces.com/problemset/problem/669/E

22.http://codeforces.com/problemset/problem/848/C

23.https://www.lydsy.com/JudgeOnline/problem.php?id=3524

24.https://www.lydsy.com/JudgeOnline/problem.php?id=1901

25.https://www.lydsy.com/JudgeOnline/problem.php?id=2674

26.https://www.lydsy.com/JudgeOnline/problem.php?id=2738

27.https://www.lydsy.com/JudgeOnline/problem.php?id=4237

28.https://www.lydsy.com/JudgeOnline/problem.php?id=2527

29.https://www.lydsy.com/JudgeOnline/problem.php?id=3110

30.https://www.lydsy.com/JudgeOnline/problem.php?id=1146

31.https://www.lydsy.com/JudgeOnline/problem.php?id=2251

32.http://tsinsen.com/A1381


【6】二进制分组算法

1.http://codeforces.com/problemset/problem/710/F

**注**：经典的强制在线ac自动机，维护一个字符串集合，支持动态插入串，动态删除串，在线查询给定串在集合中子串数目

**消除动态删除**：维护两个ac自动机森林in和out，插入串插入到in，删除串插入到out，因为此种数目满足减法性质，分别查询相减即可(代价为一个2)

**消除在线插入**：ac自动机不可在线插入串，采用二进制分组算法，在线转离线，每次插入一个串，新建一个ac自动机，阶为1，如果与上一个ac自动机阶相同，就合并到上一个，暴力重构合并之后的自动机fail树和维护的相关信息(每个串最多合并log次)，此步本质上是一种离线做法(代价为一个log)

**在线查询**：在森林中每个自动机上分别查询，叠加即可；ac自动机查询是在线的

**技巧与注意点**：

1)0号点设立为森林中所有点共用的超级虚拟节点，每个自动机空串节点插入时再自己维护

2)设S=rt[k]为第k个自动机的根，也是当前要操作的根节点，千万注意在插入完之后的构建build过程和对每个自动机的查询过程中，都要初始化一下此自动机：将0号点的每一个转移都设为S，即：go[0][c]=S

3)特别注意不要构造trie图，保留节点的每个空转移

**关于ac自动机的合并**

1)本质是DAG的合并

2)注意合并的时候，不要忘记合并节点的标记，考虑标记合并时到底是或还是加的关系，也有可能是多规则合并

**本题其他参考做法**：

1)二进制分组+后缀自动机，思路类似

2)采用分类算法，对串长设立阈值，长一点的暴力插入ac自动机中并维护，短一点的存起来暴力kmp匹配，速度较快

3)字符串hash：用到基本思想，总串长为一定规模的若干字符串，其长度种类不超过根号种

对每种长度利用一个set维护插入串的hash值，查询时扫描所有不同长度种类，再扫描此种长度的所有子串，去指定set中查询此子串hash值是否存在，其总复杂度暂不明晰

2.http://acm.hdu.edu.cn/showproblem.php?pid=4787




【分治综合训练】

1.http://codeforces.com/contest/888/problem/G

2.http://codeforces.com/problemset/problem/1140/F

注：经典的线段树分治，提取每个插入操作的存活周期，抹除删除操作

线段树标记永久化思想(一个周期分成log段)，在线段树上dfs，递归时执行插入操作，回溯时撤销

使用可撤销并查集(按秩启发式合并)，在叶节点状态回答询问

维护答案：刚开始每个横坐标和纵坐标单独一个集合，每个集合维护其中横纵坐标个数；

插入一条边，即可能合并两个集合，对答案贡献为numx[p]*numy[q] + numy[p]*numx[p]

注意撤销时的操作顺序，不要忘了维护并查集结构


【6】模拟退火算法

学习网站：http://blog.csdn.net/acdreamers/article/details/10019849
         http://blog.csdn.net/zk_j1994/article/details/53711410

1.http://poj.org/problem?id=2420

2.http://acm.split.hdu.edu.cn/showproblem.php?pid=4717

3.http://poj.org/problem?id=1379

4.http://acm.split.hdu.edu.cn/showproblem.php?pid=2297

5.http://www.lydsy.com/JudgeOnline/problem.php?id=3680

6.http://acm.split.hdu.edu.cn/showproblem.php?pid=3932

7.http://acm.split.hdu.edu.cn/showproblem.php?pid=1109

8.http://acm.split.hdu.edu.cn/showproblem.php?pid=3644

9.http://acm.split.hdu.edu.cn/showproblem.php?pid=5017

【7】bitset优化专题

1.http://codeforces.com/problemset/problem/914/F

2.http://codeforces.com/problemset/problem/1097/F

3.https://www.lydsy.com/JudgeOnline/problem.php?id=5245

【8】三分专题

1.http://codeforces.com/problemset/problem/939/E

【9】多重二分

1.http://codeforces.com/problemset/problem/965/C

【10】Method of Four Russians

[维基百科](https://en.wikipedia.org/wiki/Method_of_Four_Russians)





# 9.随机化算法

1.http://codeforces.com/problemset/problem/1091/G




# 10.分治
1.https://www.lydsy.com/JudgeOnline/problem.php?id=4449

​	给一个多边形的三角剖分，询问亮点最短路，用分治每次选一条边尽可能把两边点集分成一样大，然后裂成两个图，然后询问如果在两边肯定会结果选的边的一个端点，分别去bfs即可

2.https://www.lydsy.com/JudgeOnline/problem.php?id=2001

​	动态最小生成树，离线有分治做法，考虑如果有m条边权值不确定，图可以同过reduction和contraction操作缩减到O(m)，这样对询问序列去分治即可，这个过程和在二叉树上dfs差不多，所以直接求出下一层的边集并覆盖是没有问题的。

3.https://www.lydsy.com/JudgeOnline/problem.php?id=3897

​	应用贪心思想，每次可以抠掉最大值那个点，然后分别到两边去做，由于要查询区间最大值，所以是O(nlogn)的，可能有O(n)的做法。

4.https://www.lydsy.com/JudgeOnline/problem.php?id=2287

​	其实直接对背包做逆操作就可以了，但是像这种去掉一个点算剩下贡献可以用分治去实现。

5.https://www.lydsy.com/JudgeOnline/problem.php?id=2961

6.https://www.lydsy.com/JudgeOnline/problem.php?id=4979

​	对于全局查询有多少对区间符合一个限制，这个限制和区间端点和区间最值之类有关可以分治转成双指针维护

7.https://www.lydsy.com/JudgeOnline/problem.php?id=3745

​	求所有区间长度乘区间最大值最小值的和，分治后转为枚举一边另一边分类讨论求和

8.https://www.lydsy.com/JudgeOnline/problem.php?id=3181

​	不太算分治，就是对数据范围分类用不同的做法



# 11.交互题

1.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=10433 I题

注：与初等数论相关的概率意义下交互题，可以证明暴力的复杂度在概率意义下正确

2.http://opentrains.snarknews.info/~ejudge/team.cgi?contest_id=10433 J题

注：有趣的思维题，利用$01$串汉明距离做$2-$聚类分析，化归为简单单串情形






# 12.其他专题专项

【1】小型思维题/小型带数学证明题

1.http://codeforces.com/problemset/problem/930/A

2.http://codeforces.com/problemset/problem/940/B

3.http://codeforces.com/problemset/problem/1092/D1

4.http://codeforces.com/problemset/problem/1092/D2

注：经典问题：翻硬币，只能翻相邻两个同色的硬币，最终使得所有硬币正面朝上，或者同时反面朝上

【2】递归式处理(半数学)题

1.http://codeforces.com/problemset/problem/949/B

【3】搜索优化：dancing links精确覆盖/可重复覆盖


