# screen
---
## 缓存屏幕输出

问题描述：screen模式下，没有缓存，鼠标滚动无法查看之前的输出记录。

解决方法：

1.  在 .screenrc 文件中添加如下配置

```

# Enable mouse scrolling and scroll bar history scrolling

termcapinfo xterm* ti@:te@

```

2. 命令行启动指定文件

```

screen -c ~/.screenrc

```

3. 配置文件启动，环境变量添加如下配置

```

export SCREENRC="$HOME/.screenrc"

```

  

参考:

[在屏幕内滚动或暂停输出](https://qastack.cn/unix/40242/scroll-inside-screen-or-pause-output)

[how can I make sure my system use ~/.screenrc](https://superuser.com/questions/324310/how-can-i-make-sure-my-system-uses-the-screenrc-file)  

---