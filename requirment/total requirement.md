# Raft（有问题私我）

1. go语言学习：
   * go环境配置：
     * 下载 $\text{Goland}$
     * 下载 $\text{https://github.com/Hanyuezhuohua/Raft-2021}$（里面可能有一些不用的文件夹，不用管），并创建新的 github 仓库
     * 配置 $\text{GoRoot}$（不用配置 $\text{GoPath}$，已经配置好了 $\text{GoModule}$）
   * 语言学习:
     * https://tour.golang.org/welcome/1
     * https://go-zh.org
     * https://www.runoob.com/go/go-tutorial.html （如果实在打不开上面两个链接，不推荐）
   
2. raft资料：
   * Raft动画：http://thesecretlivesofdata.com/raft/
   * Raft论文：https://raft.github.io/raft.pdf
   * 更多内容：<https://raft.github.io>及自行上网查找。
   
3. raft实现：基于 mit 6.824 Lab2
   * 官方课程材料页：<http://nil.csail.mit.edu/6.824/2018/labs/lab-raft.html>
   * mit助教总结：<https://thesquareplanet.com/blog/students-guide-to-raft/>
   * mit助教Q/A：<https://thesquareplanet.com/blog/raft-qa/>
   * 关于锁的建议：<https://pdos.csail.mit.edu/6.824/labs/raft-locking.txt>
   * 关于raft的结构的建议：<https://zhuanlan.zhihu.com/p/103849249>

4. 测试方法：

   * 本地自己测的方法：
      * `cd Raft-2021\src\raft`
   
      * `go test`
   
      tips：由于程序本身执行顺序不一定，需要多次测试均 $\text{pass}$ 才可证明完全正确。然后我这边测试的时候也会多次测试，只要维持通过率就行。
   
     批量测试的脚本已经加入到仓库中
   
     * 使用方法：./go-test-many.sh 测试次数 并行数(默认是 CPU 个数) 哪个测试
     
       Example：./go-test-many.sh 2000 8 2C
   
   * 评测方法：由于暂时没有用于测试的OJ，我会在每个阶段的ddl把大家的仓库下下来手动评测，测试方法和大家本地测试一样。       


5. 时间安排（大致）
   * 第一周：学习go语言和raft的原理（看懂paper）
   * 第二周：完成 Lab 2(A)
   * 第三周：完成 Lab 2(B)
   * 第四周：完成 Lab 2(C)