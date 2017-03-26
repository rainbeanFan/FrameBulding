# FrameBulding

Android实际开发中的首页框架搭建
Android Studio, 框架, 结构, 首页, 实际开发, Android, Fragment切换, 设计模式

前段时间忙得不可开交，一直想抽个时间写一个博客，然后就一直拖到了现在，确实感觉有点愧疚。。。

这段时间买了几本书正在看，想让自己好好沉下心来，又去慕课网看了些视频，确实发现以前自己落下了蛮多知识点，还是有点收获，

所以，在此呼吁一下，干我们这行，需要不断学习，只有在学习中，才能明白自己有多水，才能让自己不断变强！

好了，进入正题，这一次准备了一些很基础的东西，但也是非常重要的东西，对于我们实际开发真的很有帮助

知识点一：使用BaseFragment/BaseActivity的作用：抽象到父类的思维模式

知识点二：Fragment的切换以及切换的方式

知识点三：项目结构以及命名规范

以上三个知识点，可在如下代码中一一体现

 

首先，新创建一个Android Application工程

然后创建一些文件以及包名，项目结构如下：



activity包名下严格放入Activity类，并且，都继承自BaseActivity,对于抽象到父类的思维模式可以帮我们省下很多代码，使用BaseActivity以及BaseFragment,可以将一些Activity或者Fragment的

统一操作放入父类中，比方说整个应用的SD卡业务，统一的UI修改操作，统一的权限操作，等等，反正十个App有九个是这种结构，还有一个是有问题的（慕课网老师说的，哈哈）

在这里稍微讲一下命名规则，如果公司没有指定的一套命名规则的话，以上的命名规则对于实际开发确实很有帮助，是Actiivty的，以Activity结尾，是Fragment的，以Fragment结尾，

布局文件是Activity的布局，以activity开头，layout结尾，中间为具体的业务名称

Fragment的布局与Activity一样，以fragment开头，以layout结尾，中间是具体业务的名称

这样对于后期浏览的时候，能够一目了然
