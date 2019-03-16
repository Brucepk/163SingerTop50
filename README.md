# Python爬虫爬取网易云音乐各类型歌曲的50大热门歌手名单

### 本代码文章首发于公众号「Python知识圈」，如需转载，请通过公众号联系作者pk哥，谢谢

![公众号](https://github.com/Brucepk/pk.github.io/blob/master/gzh.jpg)

#### 公众号里提供了我的微信，可以联系到我。

半个月前和媳妇一起去梅赛德斯－奔驰文化中心听了一场 Angela 张韶涵的演唱会，主要是我媳妇是她的粉丝，从小都喜欢她的歌，还凭借她的歌拿到过校园十大歌手比赛的前三名。渐渐的，我也成了她俩的歌迷，哈哈。演唱会开场第一首歌就用了很震撼的「呐喊」，前奏还加了重金属的元素，加上 Angela 清亮的高音，让整首歌听起来更加热血沸腾。本想跟着一起「呐喊」，无奈自己歌词记不住。所以想着用 Python 爬虫写一个网易云音乐的系列。先从基础的爬取歌手的姓名的歌手 id ，之后根据 id 再爬虫歌手名下的歌曲歌词和歌曲评论。

今天就先带大家爬取网易云音乐下的歌手信息并把数据保存下来。


##### 爬取结果

![爬取结果](https://github.com/Brucepk/pk.github.io/blob/master/ms1.jpg)



#### 环境

语言：Python
工具：Pycharm

#### 导包
BeautifulSoup：用来解析源码，提取需要的元素。

selenium：因为歌手信息不在页面源代码里，用 selenium 自动化测试库直接获取调试页面的 Elements 元素信息。

csv：数据以 csv 形式保存下来。

全部文章请[点击这里查看](https://mp.weixin.qq.com/s?__biz=MzU4NjUxMDk5Mg==&mid=2247484004&idx=1&sn=65bd49e9ece828bb2b1bbf9041c4d8b8&chksm=fdfb659bca8cec8da621ecdf7fdd77dca4af6278ba640009d9a5f5b43df117a58a28c23c87ef&token=1092009955&lang=zh_CN#rd)
