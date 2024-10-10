# mpv播放器配置

本项目为不同的平台采用不同的分支命名，这么做的原因是有些脚本对应不同系统的文件目录有所差别，所以为了保证直接拉取的可用性，所以这么设置。


## 使用方法

- main 分支，windows 平台使用


```
cd you_mpv_home_path # 修改为自己mpv所在目录
git clone https://github.com/muyiacc/mpv-config.git portable_config
cd portable_config
```

- linux 分支，linux 平台使用

```
cd ~/.config/mpv
git clone https://github.com/muyiacc/mpv-config.git .
git checkout linux
```

## 快捷键

这里记录的快捷键非通用，而是本项目安装的第三方脚本自定义的快捷键，也有很多是脚本的默认的。

| 快捷键 | 依赖的脚本 | 说明 |
| --- | --- | --- |
| a | [thumbfast](https://github.com/po5/thumbfast) | 手动触发缩略图加载|
| y | / | 旋转视频，默认快捷键没有
| ctrl+o | [mpv-file-brower](https://github.com/CogentRedTester/mpv-file-browser) | 打开文件浏览 |
| `（英文下的飘号，左上角） |  [recent](https://github.com/hacel/recent) | 打开最近播放 |

## 脚本
| 脚本 | 说明 |
| --- | --- |
| [autoload](https://github.com/mpv-player/mpv/blob/master/TOOLS/lua/autoload.lua) | 自动播放下一集 |
| [mpv-file-brower](https://github.com/CogentRedTester/mpv-file-browser) | 文件浏览器，可在mpv切换目录选择文件播放 |
| [recent](https://github.com/hacel/recent) | 最近播放，可通过 ` 快速打开最近播放的历史文件|
| [thumbfast](https://github.com/po5/thumbfast) | 进度条缩略图 |

