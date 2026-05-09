最近使用有使用远程SSH修改代码并且要沿用自己的SKILL的需求, 但是没有claude cli没有ssh功能, 于是寻求一种间接的访问方式.

在伟大的KIMI 2.6大人的教诲下, 发现Zed是一个完美的解决方案

首先, Zed支持Remote SSH, 能实现远程修改代码

最重要的是, Zed可以直接使用Claude Cli

配置方式如下: (MacOS)

进入 ~/$HOME/.config/zed/settings.json (这是Zed的全局配置窗口)

添加:

"agent_servers": {
    "claude":{
      "env": {
        "CLAUDE_CODE_EXECUTEABLE": "/Users/racolw/.local/bin/claude"
      }
    }
  }

然后打开Zed, 在里面打开Agent窗口, 改为Claude就行了.

###前置需求

Claude Code 已经安装并且配置

Zed 以及安装
