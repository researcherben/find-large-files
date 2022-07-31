The Jupyter Notebook produces a histogram of file sizes

Below are related topics

# find large files

The following works on CentOS but not MacOSX
```bash
find . -printf '%s %p\n' 2> /dev/null | sort -nr | head -n 100 > filename.log
```

# folder size sorted (top-level only), round up to kilobytes
```bash
du -cks * | sort -rn | head -11
```

```bash
du -h /home | sort -rh
```


# ncdu - NCurses DU = terminal-based interactive navigation

<https://dev.yorhel.nl/ncdu>

can be run offline: <https://stackoverflow.com/a/16564104/1164295>

# qdirstat - GUI
from author of KDirstat
<https://github.com/shundhammer/qdirstatL>

Can load data from from scripted output
<https://github.com/shundhammer/qdirstat/blob/master/doc/QDirStat-for-Servers.md>  
<https://github.com/shundhammer/qdirstat/tree/master/scripts>

# command-line histogram

<https://unix.stackexchange.com/questions/177777/drawing-a-histogram-from-a-bash-command-output>

<https://github.com/glamp/bashplotlib>
