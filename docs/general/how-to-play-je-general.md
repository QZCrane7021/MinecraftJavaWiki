# 入坑 Minecraft Java 版 — 基础

## 运行原理

和大多数游戏不同，Minecraft Java 版并没有可执行文件，而是一个 `.jar` 包。`.jar` 包由 Java 字节码打包而成，需要 JRE（Java Runtime Environment，Java 运行时环境）才能执行。而这个 JRE，如果搜索渠道错了，很可能下载到的不是安装程序而是源码包，需要手动放入硬盘某处、添加 PATH 环境变量，相当麻烦，因此 Java 版的入坑门槛相当高。

所幸，市面上有一些第三方的 “启动器”，可以快捷管理、启动 Minecraft Java 版的实例，有些启动器还兼具自动下载、配置 JRE 的功能。

!!! tip "JRE 和 JDK"
    JDK 是 Java Developer Kit，Java 开发者套件的简称。乍一看，玩家根本不需要开发者功能，明显不该下载 JDK。但是，JDK 必然内置一个 JRE，而自 Java 11 版本起，Oracle 公司就不再分发单独的 JRE。考虑到新入坑的玩家一般都会直接选择高版本，而高版本一般都需要 17、21 甚至 25 版本的 Java，几乎可以说，新玩家无需认识 JRE，直接下载配置 JDK 即可。

## 版本选择

MC 的版本茫茫多，该怎么选择？

对于新入坑的玩家，一般不建议贸然尝试低于 1.12 的版本。新玩家就算暂时不想引入大型的玩法类模组，也大概率需要辅助类模组，因此还是建议挑选模组较为丰富的版本。具体来说，建议使用：

- 1.20.1 + Forge 加载器
- 1.20.1 + Fabric 加载器
- 1.21.1 + Neoforge 加载器
- 1.21.1 + Fabric 加载器
- 1.21.11 + Fabric 加载器

## 启动器

虽然许多老玩家推荐 HMCL 启动器，但对于新玩家，还是建议 Plain Craft Launcher（简称 PCL）或者 PCL Community Edition（简称 PCL-CE 或 PCL 社区版）。需要注意，这两个启动器及前文的 HMCL 都在 Github 上开放了部分或全部源代码，软件本身是免费的，**千万不要上当受骗，购买所谓的 “付费版”！**

[下载 HMCL][download-hmcl]|[下载 PCL][download-pcl]|[下载 PCL-CE][download-pcl-ce]

[download-hmcl]:https://hmcl.huangyuhui.net/download/
[download-pcl]:https://ifdian.net/p/0164034c016c11ebafcb52540025c377?_gl=1%2akd252y%2a_ga%2aMTM5Nzc3NjgyMy4xNzY5Njc3MTUw%2a_ga_6STWKR7T9E%2aczE3NzgyNDkzMTckbzIkZzEkdDE3NzgyNDkzNDgkajI5JGwwJGgxNTQwOTQ5NTA3
[download-pcl-ce]:https://www.pclc.cc/projects/pcl-ce/#%E8%8E%B7%E5%8F%96

## JDK

用 PCL 启动，如发现缺少对应版本的 JDK，会自动下载配置。同一版本的 JDK，各家会调校发行不同的具体版本，有些版本据说性能更好（例如 Graalvm），但不明确。一般来说，PCL 自行补全的 JDK 就足够了。