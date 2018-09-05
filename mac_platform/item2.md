1. 安装[iterm2](https://www.iterm2.com/)然后打开;

2. 安装oh-my-zsh
```
curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh
```

3. 安装powerline
    - 确保安装了pip：`sudo easy_install pip`
    - 执行：`pip install powerline-status`
    - 如果安装遭遇权限问题导致安装失败，则执行：`pip install powerline-status --user -U`

4. 下载、安装字体库
    - 下载[字体库](https://github.com/powerline/fonts)，然后cd到该目录下；
    - 安装字体库，执行`./install.sh`，安装完成后提示所有字体均已下载到/Users/superdanny/Library/Fonts路径下

5. 设置iterm2的 regular font 和 non-ASCII font: Profile -> Text。推荐12pt Meslo LG S DZ Regular for Powerline

6. 安装[solarized配色方案](https://github.com/altercation/solarized)。进入刚刚下载的工程的solarized/iterm2-colors-solarized 下双击 Solarized Dark.itermcolors 和 Solarized Light.itermcolors 两个文件就可以把配置文件导入到 iTerm2 里。

7. 使用agnoster主题
    - 下载[agnoster主题](https://github.com/fcamblor/oh-my-zsh-agnoster-fcamblor),到下载的工程里面运行install文件,主题将安装到`~/.oh-my-zsh/themes`目录下
    - 设置该主题。进入~/.zshrc打开.zshrc文件，然后将ZSH_THEME后面的字段改为agnoster。ZSH_THEME="agnoster"（agnoster即为要设置的主题）

8. 增强指令高亮效果（当用户输入正确命令时指令会绿色高亮，错误时命令红色高亮）：
    - cd到.zshrc所在目录
    - 执行指令将工程克隆到当前目录:`git clone git://github.com/zsh-users/zsh-syntax-highlighting.git`
    - 打开.zshrc文件，在最后添加下面内容:`source XXX/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh`，保存文件。注意：xxx代表.zshrc所在目录
    - cd ~/.oh-my-zsh/custom/plugins
    - 再次打开.zshrc文件，在最后面添加下面内容`plugins=(zsh-syntax-highlighting)`，保存文件。



最终效果还是可以的：
![1d71ce2f889098ff.png](file:///Users/tristanhuang/Desktop/myTerminal/mac_platform/images/1d71ce2f889098ff.png)


--------- 
1. 我的agnoster主题有点问题，就是提示符的那个箭头出不来，是问号一样的东西，所以试了一下还比较好的主题有：sunrise/sunaku/wezm
2. 查看系统当前支持的shell:`cat /etc/shells`

---------
参考的地方：
1. [iterm2 && Oh My Zsh](https://www.jianshu.com/p/7de00c73a2bb)
2. [强大的终端工具ohMyZsh](http://www.itboth.com/d/vii6vv/linux)