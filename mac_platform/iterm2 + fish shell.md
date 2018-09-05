1. `brew install fish`
2. `sudo vim /etc/shells`，添加最后这一行
  ```
  # List of acceptable shells for   chpass(1).
  # Ftpd will not allow users to connect who are not using
  # one of these shells.

  /bin/bash
  /bin/csh
  /bin/ksh
  /bin/sh
  /bin/tcsh
  /bin/zsh
  /usr/local/bin/fish
  ```
  
3. `chsh -s /usr/local/bin/fish`，切换shell到fish


------------
常用快捷键：
1. 自动建议
Fish 会自动在光标后面给出建议，颜色为灰色。按下→或Control + F表示采纳建议，按下Alt + →表示只采纳一部分。
2. Tab 键补全
按下 Tab 键，Fish 将尝试自动补全命令、参数或路径，如果有多条补全建议，可以继续使用 Tab 键在不同建议间切换。
