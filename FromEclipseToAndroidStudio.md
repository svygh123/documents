#AndroidStudio比Eclipse好用在哪里

* **Android Studio是一个全新的基于`IntelliJ IDEA`的Android开发环境。  **
+ __Android Studio提供了集成的Android开发工具用于开发和调试，自动化构件工具也集成了。  __
- __Android Studio2.0预览版已经出来了，已经比较稳定了。__

下面列举来一下AndroidStudio有的eclipse没的，下面的功能eclipse基本上没有，不过不代表有的就一定是好的，但是有这些东西了，还运行得那么快，那就不得不佩服了：

1. 自动保存功能，再也不用频繁的戳`Ctrl+S`了，因此S在这里是`Setting`的简写。
2. 鼠标移到左侧滚动条，有预览该处的代码矩形框，再也不用拖动滚动条了，移动鼠标即可。
3. 左/右/下区域框自动隐藏设置，点击区域框右上角的设置图标，将Docked Mode去掉勾选。
4. 自带团队开发工具：GitHub,CVS,Git,Google Cloud,Mercurial,Subversion。
5. 自带自动化构件工具：Maven,Gradle。
6. 可以直接导入在GitHub上托管的开源项目：File->New->Project from Version Control->GitHub
7. 快捷键设置：`Ctrl+Alt+S`(`Setting`)->Keymap(eclipse是没有Preference快捷键的)，在搜索框按照字面意思输入大概的英文，如delete，就实时看到有关删除的一些快捷键，假如不知道某个快捷键代表什么呢，那么可以把鼠标移到搜索框后面的搜索图标，就会看到Find Actions By ShortCut，意思就是根据快捷键搜索，单击一下，会出现输入框，可以随便按一个组合快捷键如`Ctrl+D`，就会有相关结果实时列出，多么懂程序员的搜索功能呀，明白了以后，想从eclipse或其他开发工具转android studio的同学，就可以将之前在eclipse或其他开发工具的快捷键在这里试试看有什么区别，如果不想学习新的快捷键呢，那么好，请看Keymap:右边的下拉框，这里列出了N多个开发工具的快捷键，选一下，就瞬间回到了那个开发工具的快捷键模式了，学习成本瞬间降到负数。
8. Android Monitor，实时动态无刷新自右向左滚动显示：Memory(内存)/CPU(中央处理器)/GPU(图形处理器)/Network(网络)  这些在计算机的使用情况。
9. 捕获快照。有时候我们的服务器突然就死机了或者登陆不上了，这时候我们就要监控java堆和内存分配情况，而捕获快照就是捕获监控过程保存下来然后分析。java堆捕获快照方法是单击Android Monitor里面的![heap dump](images/studio-dump-heap-icon.png "heap dump")，然后在左侧区域的Captures页签能看到Head Snapshort下的子节点就是我们保存的捕获到的java堆快照，然后你就可以分析了，你也可以导出这个文件，右键Export to standard .hprof；内存分配情况捕获快照方法是单击Android Monitor里面Memory页签的Start/Stop Allocation Tracking图标![memory allocation](images/studio-allocation-tracker-icon.png "memory allocation")，是区域捕获，所以要点一次开始，然后点一次结束，捕获一段快照，然后在左侧区域的Captures页签能看到Allocation Tracking下的子节点就是我们保存内存分配情况快照，这个不用导出，直接右键该文件->`Show in Explorer`就能得到这个文件了。
10. 异常提醒及跳转精确到光标列位置。如TypeError: Cannot call method 'init' of undefined at Object.init (file:///android_asset/www/js/factory.js:136:35)，相信这种异常不会陌生吧，接下来就打开factory.js然后定位到136行35列，怎么快捷定位呢，用快捷键，打开资源文件在Android Studio里面是`Ctrl+Shift+N`，而Eclipse里面则是`Ctrl+Shift+R`，打开了吧，定位到行列在Android Studio里面是Ctrl+G(Excel也是这个)，而Eclipse里面则是`Ctrl+L`，这太麻烦了吧，要用2次快捷键，其实可以用一次的，直接复制`factory.js:136:35`然后`Ctrl+Shift+N`，如果搜索结果在第一个，直接再回车，而且在输入过程中不卡顿，Android Studio想的真周到。关于这2个工具的快捷键对照，已有文章专门列举。
11. 未完待续......

