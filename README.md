# Joyful-Pandas
<img src="picture/panda.jpeg" width="240" height="高度" alt="图片名称" align=center>

#### 一、写作初衷

在使用Pandas之前，几乎所有有关的大型表格的处理我全部用xlrt和python循环来实现，基本上这已经几乎能做一切事情了，但显而易见的缺点：慢！稍微复杂一点的逻辑就不得不写很多效率奇差的代码（水平糟糕的表现），而且可复用性几乎为零，即处理了这个表格的代码不太可能再取处理其他的表格。

曾经也尝试过使用Pandas，但是当时就是零零碎碎地去学，学完就忘，一周过去了啥也不会了，这也是这个包很大的一个特点，Pandas绝对不是一个Toy Package，里面有十分丰富的内容，每个函数的参数可选项也巨多，因此也同时变得巨麻烦，报错是常有的事，过了一会自信就被打击了。

上个学期的期末考试前，我偶然找到了一本全部讲Pandas的神书（即Theodore Petrou所著的Pandas　Cookbook，可在网上下到pdf，不过现在还没有中文版），寒假开始后立即快速地过了一遍，发现之前很多搞不清的概念得到了较好的解答，逐步地再对着官方文档一字一句查看，最后总是建立了大的一些宏观概念。

综上，开始这个项目的理由大致如下：

１、完整梳理Pandas的主线内容，基本覆盖官方手册的主要内容和常用知识点。

２、国内单独讲Pandas的书籍较少（见到最常用的应该是《利用Python进行数据分析》和《Python数据科学》两本书，可能其他书也会部分提及），网络资料零碎，体系性较差。

３、学习Padans是典型的任务驱动型的过程，在每一块内容都设计了对应的综合运用，将所学运用到实际（包括我之前遇到过的所有困难的例子，见第9章），树立”xlrt能解决的问题，Pandas能解决得又快又好“的观念，增强信心，从Painful-Pandas转变为Joyful-Pandas。

#### 二、编排思路与内容

本项目共有九章，可以大致分为4个板块：

１、拿到数据必然先要读取它，分析完了数据必然是要保存它，读取了数据之后，我们面对了怎样的对象（Series? of Dataframe?）是第一重要的课题，因此了解序列和数据框的常规操作及其组件（component）便是必须涉及的内容。此外，多层标签/索引/列往往会使我们烦躁，这是因为我们还不够了解它，我想看完了第一章，你和它们会像老朋友一样受熟悉。

２、对于一个DataFrame而言，如果一个操作使得它的元素信息减少了，那就对应了索引，即第二章的内容；如果这个操作使得数据的信息被充分地使用，那有两种可能，第一是数据被分组，从组内提取了关键的信息，第二就是数据呈现的结构或形态上的变化，使得我们更容易地能够地进一步处理数据，这两者分别对应了第三章与第四章的内容；最终如果一个操作使得原本不属于这个数据框的信息被加入了进来，那往往是涉及到了合并操作，对应了第五章的内容。从数据信息增减的角度，拆解成了3个板块，4个章节，几乎串联其了官方文档关于数据框操作的全部内容，我想这样的安排是合适的。

３、如果说前面我们关心了序列和数据框这两种容器的结构和操作，那么下面就要关心其中的元素，特别地，我们将在第六章涉及到分类变量、缺失型变量和文本型变量，第七章涉及到文本型变量，第八章涉及到Pandas中的Plot模块（图可以看做元素的某种呈现）。

４、正如前面所说，Pandas的学习往往是任务驱动型，一个操作或者某个方法，不去使用自然会很快地忘记（除非你天赋异禀！那我推荐直接阅读那一堆官方文档），因此我在每一章（除了第一章）都会添加“问题和练习”的部分。其中，问题中出现的往往是对于教程中某个细节的深入，或者在这一个章节中重要的函数，希望你能够查阅相关资料阅读以解决问题；而练习部分包含了两个综合题，分别是两个不同的案例，相当于对前面所学知识的考察与综合运用，虽然并不是非常复杂，但是想要全部完成，的确是要动不少脑筋才行。最终，在第9章中会添加若干个我曾经遇到过但解决方案复杂，或者我想到的某一个一时半会儿还没有解决办法的问题，具有一定的挑战性，如果有较好的解决方案，欢迎交流分享，谢谢：）

最后，祝你有所收获！

#### 三、版本要求

１、Pandas于2020年1月29日发布了1.0.0的版本，本项目全部使用新版本

```
Python: 3.6+
Numpy: 1.17.4
Pandas: 1.0.0
Matplotlib: 3.1.2
```

#### 四、反馈

１、欢迎任何有益的建议或想法，可邮件(1801214626@qq.com)交流！

２、不免有错误，欢迎提Issues！
