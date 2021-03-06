# 正交性：
**什么是正交性：在几何学中，如果两条直线相交成直角它们就是正交性。在计算机技术中，表示某种不相依赖或者是解耦。如果两个或者更多个事物中的一个发生变化，不会影响其他的事物，这就叫正交性**

### 知识要点：
> * 在任何系统中，各个组件都高度依赖，就不再会有局部修正这样的事。

> * 我们要设计自足的组件：独立，具有单一，良好定义的目的，称之为内聚。

> * 与编写单个的大块代码，编写多个相对较小，自足的组件更为容易，也更好维护。

> * 正交的途径还可以促进服用。如果组件具有良好，明确，具体定义的责任，就可以用最初未曾想过的方式与新组件进行组合。

> * 正交使系统更加的健壮，对特定的区域进行细微的修正或者改动，你所导致的问题都会局限在特定的区域中，不会把问题暴露在外部。

> * 使用正交性，你不会与特定的供应商，产品，或是平台紧绑在一起，因为这些第三方接口将被隔离在全部开发的较小部分中（ps:如何去隔离这些第三方的接口，或者与第三方的对接的更改，我自己还是没有找到好的办法。在过去的项目中有很多需要是要我们配合第三方或者特定的产品进行改动，如何才是隔离在较小的部分而不去影响正常的功能？)

> * 你是否注意到，有些团队很有效率，每个人都知道做什么。而另一些团队却不停的在争吵而且无法避免互相干扰，每一次改动都需要全团队人开会，因为一次修改他们中的任何一个人都会受到影响。（ps:怎么像我现在团队？：（ ）这时候就需要分工明确，如果每个人写的代码都符合正交性，这样一个改动可能会影响到的其他人员就比较少。

> * 从设计的方面，系统应该是由一组相互协作的模块组成的，每个模块都实现不依赖其他模块的功能（ps:这里应该是MVC的设计思想吧）

> * **一旦设计好组件，这时候你就要问问你自己：“一旦显著的更改了某个功能背后的需求，会有多少个模块受到影响？”在正交系统中，答案应该是一个。（在现实中这显得很天真，很难做到，但是你根据功能的分析变动，每个功能的变动在理论上应该是一个。我的理解就是，自己设计的模块，应该在任何的变动下，影响到其他模块的可能降低到最小）**

> * 在编码的时候如何使用正交：1. 让你代码保持解耦。2.避免使用全局的数据。3. 避免编写相识的函数。

> * 重复的代码是结构问题的一种症状。要了解更好的实现请看设计模式这本书（ps:这是我下一本需要学习的书） 

> * **养成不断地批判对待自己代码的习惯。寻找任何重新进行组织，以改善其结构和正交性的机会。这个过程叫做重构**

紧密的结合DRY原则，运用正交性，你将会发现你开发的系统会变得更加的灵活，更易于理解，并且更易于调试，测试和维护。

### --挑战
1. 考虑常在windows系统见到的面向GUI的大型工具，和在shell提示下使用的短小却可以组合的命令行工具。哪一种更为正交，为什么？如果正好按其设计用途加以应用，哪一个更易于使用？哪一种更易于与其他工具组合满足新的需求？
> 暂时这些工具都没有使用过，现在还回答不上来

2. C++支持多继承，java允许类实现多个接口。使用这些正交性有何影响？使用多继承和多接口影响是否不同？使用委托和多继承之间是否不同
> 暂时只会PHP语言，希望以后能回答这些问题。

&emsp;&emsp;--回答时间：2017.12.17