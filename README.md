# 火光摇曳

### 下载编译好的版本

1. 查看 release 目录获取编译好的版本
2. 这里下载：http://pan.baidu.com/s/1V77Vg

### 自己编译这本书？
* Win

  安装CTex-full, 打开 main.tex,  通过 XeLatex 编译。 

* Linux & Mac 

  $>  xelatex main.tex


### 编译出错 ？

* Win
 
  确认在UTF-8 编码下打开通过 CTex 下的 WinEdt 打开 main.tex， 点击对应的 XeLatex 按钮进行编译。如果安装的 CTex-full 完全版，则缺省字体都支持。 

* Linux & Mac 

  编译前预计需要配置一下XeLatex 字体， 配置过程参考 http://www.douban.com/note/322135009/

  我目前的XeLatex 字体配置文件： /usr/local/texlive/2013/texmf-dist/tex/latex/ctex/fontset/ctex-xecjk-winfonts.def
    
      % ctex-xecjk-winfonts.def: Windows 的 xeCJK 字体设置，默认为六种中易字体
      % vim:ft=tex
      \setCJKmainfont[BoldFont={SimHei},ItalicFont={KaiTi_GB2312}]{SimSun}
      \setCJKsansfont{SimHei}
      \setCJKmonofont{FangSong_GB2312}
 
      \setCJKfamilyfont{zhsong}{SimSun}
      \setCJKfamilyfont{zhhei}{SimHei}
      \setCJKfamilyfont{zhkai}{KaiTi_GB2312}
      \setCJKfamilyfont{zhfs}{FangSong_GB2312}
      \setCJKfamilyfont{zhli}{LiSu}
      \setCJKfamilyfont{zhyou}{YouYuan}

      \newcommand*{\songti}{\CJKfamily{zhsong}} % 宋体
      \newcommand*{\heiti}{\CJKfamily{zhhei}}   % 黑体
      \newcommand*{\kaishu}{\CJKfamily{zhkai}}  % 楷书
      \newcommand*{\fangsong}{\CJKfamily{zhfs}} % 仿宋
      \newcommand*{\lishu}{\CJKfamily{zhli}}    % 隶书
      \newcommand*{\youyuan}{\CJKfamily{zhyou}} % 幼圆

      \endinput
              

### FAQ

* 看到某些图片覆盖了一些文字？ 

  目前在 Win 下用 CTex 编译的时候不会出现这个情况。 但是在 Linux & Mac 下编译的时候， 会出现某些图片覆盖文字的情况。 如果把图片转换为 eps 格式，再进行编译则不会出现这些问题。 是否有更好的解决方案，请Latex高手指点。 

