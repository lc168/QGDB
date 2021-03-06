#                                                   QGDB
## 你为什么会看到这个github？
>因为每个c/c++人心中都有梦想。成为最优秀的c/c++程序员。

>到现在为止，最阻碍我的问题，其实是当面对，lwip，uboot，kernel，busybox，STL，caffe，Qt，opencv, ffmepg 这样c/c++优秀开源项目的时候，我们总有入宝山而两手空空的感觉。

>对于这些优秀的开源项目，你可以在很短时间（比如3天）就掌握这些开源项目的精华，我想我们自然就是高手了。
>这就是为什么你会看到这个github项目了。

## 那么如何在很短时间内就掌握，你想掌握的c/c++开源项目呢？
>我的解决方案。是构造一个高级的gdb调试工具。

>将整个代码的数据结构都绘制出来，随着代码调试， 用图画的形式，直观的展示，数据结构的变化的过程。

>程序 = 数据结构 + 算法。

>数据结构我们绘制，算法实际上就是数据变化的过程。
>于是最终希望代码走读过程像放电影一样，清晰展现。

>并且要把gdb的反向调试功能加上，让数据过程可以逆流。

（不懂“反向调试的”可以看看这个
https://sourceware.org/gdb/current/onlinedocs/gdb/Reverse-Execution.html#Reverse-Execution，
反向调试可以说是神技了吧？）

## 为了达成这个目标那么我做过哪些努力呢？
实际上我有这种想法已经，2年了。做了很多努力。但是确实没有成功

>比如：开始去学习：《flex&bison》《自己动手做编译器》《自制编程语言》
>但是发现，这些基本上都是，做的一些玩具编译器，真正的c/c++还是用不上。失败了

>比如：去学习clang/LLVM， 但是门槛太高无法掌握。失败了

>比如：去研究vscode，想找到合适的vscode插件。也失败了

>比如：使用cgdb 和 DDD这种图形化的调试工具。 但是cgdb感觉还是无法达到看到数据流动变化的效果。  DDD又bug太多，无法使用。也失败了

>2年过后，我觉得，我无法一个人完成项目，于是决定，开始
>去csdn，知乎， 微信，qq，今日头条，去散发这个项目，
>希望大家可以在GitHub上面多给我一些建议。

# 目前项目进展

### 2020年3月15日 现在我在思路明确了。 
>**要控制gdb来获取，调试程序的数据，并且把数据过程用，Qt绘制出来。**   
>我最近刚刚开始学习Qt。Qt绘图不算复杂。 但怎样用gdb获取调试程序的数据结构和变化过程这个是关键？ 
>目前我明确知道，需要使用 gdb/MI接口，但是具体怎么使用gdb/MI接口我还没有头绪。

