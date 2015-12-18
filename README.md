# 火光摇曳

### 下载编译好的版本

查看 release 目录获取编译好的版本

### 自己编译这本书？
Linux & Mac 下

$> xelatex main.tex

Windows 下使用 CTex 编译，有可能要修改一下字体配置文件

### 编译出错 ？

编译前预计需要配hi一下字体， XeTex & CTex 的字体配置，配置过程参考 http://www.douban.com/note/322135009/

XeLatex 字体配置文件： /usr/local/texlive/2013/texmf-dist/tex/latex/ctex/fontset/ctex-xecjk-winfonts.def
    
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
              

