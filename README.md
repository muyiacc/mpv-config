# mpv播放器配置

本项目为不同平台提供了不同的分支配置，目的是为了适配各系统的文件目录差异，确保用户可以直接拉取并使用。

## 使用前须知

如果你想对配置进行自定义修改，可以先 fork 本项目，然后基于你的需求进行调整后再使用。

## 使用方法

### Windows 平台
适用于 `main` 分支。请按照以下步骤操作：
1. 打开终端，进入你的 mpv 安装目录：
   ```bash
   cd <you_mpv_home_path> # 将路径替换为你的 mpv 安装目录
   ```
2. 克隆本项目到 `portable_config` 文件夹：
   ```bash
   git clone https://github.com/muyiacc/mpv-config.git portable_config
   ```

### Linux 平台
适用于 `linux` 分支。请按照以下步骤操作：
1. 创建 mpv 配置目录（如果尚未存在）并进入：
   ```bash
   mkdir -p $HOME/.config/mpv && cd $HOME/.config/mpv
   ```
2. 克隆本项目到当前目录：
   ```bash
   git clone https://github.com/muyiacc/mpv-config.git .
   ```
3. 切换到 `linux` 分支以应用对应配置：
   ```bash
   git checkout linux
   ```

## 快捷键说明

以下列出的是本项目安装的第三方脚本所自定义的快捷键，以及部分默认快捷键的功能说明。更多 mpv 默认快捷键可参考：[mpv快捷键](https://blog.seektao.cc/p/241009155809/)。

- **a**  
  依赖脚本：[thumbfast](https://github.com/po5/thumbfast)  
  功能：手动触发缩略图加载。

- **y**  
  功能：旋转视频。此功能为项目新增，默认快捷键未提供。

- **Ctrl+o**  
  依赖脚本：[mpv-file-browser](https://github.com/CogentRedTester/mpv-file-browser)  
  功能：打开文件浏览器，用于切换目录或选择文件播放。

- **`（英文下的飘号，左上角）**  
  依赖脚本：[recent](https://github.com/hacel/recent)  
  功能：打开最近播放的历史文件列表。

## 脚本说明

以下是本项目中包含的主要脚本及其功能描述：

- **autoload**  
  来源：[autoload](https://github.com/mpv-player/mpv/blob/master/TOOLS/lua/autoload.lua)  
  功能：自动播放下一集视频，适合连续剧或系列文件的播放场景。

- **mpv-file-browser**  
  来源：[mpv-file-browser](https://github.com/CogentRedTester/mpv-file-browser)  
  功能：提供文件浏览器功能，允许在 mpv 中切换目录并选择文件播放。

- **recent**  
  来源：[recent](https://github.com/hacel/recent)  
  功能：记录最近播放的文件历史，支持通过快捷键 ` 打开历史列表。

- **thumbfast**  
  来源：[thumbfast](https://github.com/po5/thumbfast)  
  功能：在进度条上显示缩略图预览，提升视频浏览体验。