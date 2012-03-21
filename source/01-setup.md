# 安装与配置

你有志于成长为一名忍者，很好，那么首先去把火影看完了再来看这本秘笈吧。

当然，不看火影也没关系。咦，怎么有些观众朋友真的离场了？剩下的朋友就别去叫他们了。R这货，是统计学家为统计学开发的一套数据杀器，但那只是对下忍的介绍，对一名上忍来说，必须对它有更全面的认识，否则你查克拉再强、分身再多，在执行任务时也可能会被各种与统计无关的细节给缠死。R的安装有专门的手册，名曰_R Installation and Administration_，我就不说它在哪儿了，你也别问我要，如果你真的那么感兴趣，请自己去找。

哎哎，怎么又有几位客官走了？其实不用这么听话的，忍者得有自己的判断。我不说的原因是R官方的所有手册基本上都很坑爹，R核心团队都是写代码的高手，可是手册写出来都让人昏昏欲睡，一点读的欲望都没有，这样也好，让他们专注于代码开发吧。迄今为止，我唯一看的手册是_Writing R Extensions_，因为我需要写R包，不按它来就没法整；官方手册技术性太强，这也给无数作者创造了写作机会，不然你也不会看到这里来。

## 安装R

R的首页在<http://www.r-project.org>，你打开之后一定很失望，苍天呐，世上怎么还有这么古董的网站！几乎是纯文本网站（高级码农都这德行），首页上的那幅图已经七八年没换过了，还用着古老的框架技术。算了，不吐槽了，下载链接在左侧，写着CRAN的那地方。你是忍者，所以你当然不能直接去下载就完事，你得了解CRAN（Comprehensive R Archive Network）这一套东西。所谓的C什么AN是自由软件世界常见的软件分发方式，类似的还有为TeX准备的CTAN，为Perl弄的CPAN等。Linux打一出生就是通过网络发布的，直到今天这个特性还是没有变，后面再详谈Linux的问题。Archive Network的大意是这软件有个主服务器，然后在世界各地有一些镜像服务器，上面的文件和主服务器保持同步，这样减轻主服务器的下载压力，并让其它地区的用户能有更快的下载速度（从离自己近的本地服务器下载）。R除了自己的主程序，还有三千多个用户贡献的附加包，以及各种文档，这一大箩筐东西被复制到世界各地几十台服务器上供用户下载。

你是中国用户，可以选一个国内的镜像。这里我们要特别感谢那些志愿提供服务器的单位对自由软件的支持。

- Windows
  - 去掉安装目录中的版本号
  - 避免中文目录
- Linux
  - Ubuntu可以设置软件源
  - 尽量避免./configure & make，但这玩意儿你最好会
- Mac OS
  - 打包好的

坑爹的程序包导航（Task View），你找得到它吗？R core的答复让人很桑心。

## 配置R

`.Rprofile`文件

`.Renviron`文件
