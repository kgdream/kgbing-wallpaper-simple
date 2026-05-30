# kgbing-wallpaper-simple
极简黑白线条风格的 Bing 壁纸切换工具。
# KGbing Wallpaper Simple

极简黑白线条风格的 Bing 壁纸切换工具。  
一键获取并设置每日 Bing 壁纸，支持定时自动更换、画报模式、空闲自动切换等功能。

## 功能

- 一键获取并设置今日 Bing 壁纸
- 定时自动更换壁纸（可配置间隔时间）
- 画报模式（定时切换本地壁纸）
- 空闲自动画报模式（检测到用户空闲后自动切换）
- 壁纸历史浏览和管理
- 自动删除旧壁纸（节省内存）
- 系统托盘图标，方便快捷操作
- 开机自启
- 自定义壁纸存储路径
- 网络代理设置
- 多语言支持

## 运行环境

- Python 3.6 或更高版本
- 操作系统：Windows（主平台）

## 依赖
PyQt5>=5.15.0 Pillow>=10.0.0 pystray>=0.19.5


Plain Text


## 快速开始

### 从源码运行

1. 克隆或下载本仓库。
2. 进入 `源代码` 目录。
3. 安装依赖：

```bash
pip install -r requirements.txt


Plain Text


4. 运行程序：

```bash
python main.py


Plain Text


### 使用已打包的 EXE

1. 下载 `dist/KGbing Wallpaper Simple.exe`。
2. 双击运行即可。

## 配置说明

配置文件 `config.json` 与程序同目录，内容示例：

```json
{ "auto_change_enabled": true, "auto_change_interval": 60, "slideshow_interval": 30, "idle_slideshow_enabled": false, "idle_slideshow_timeout": 5, "auto_delete_old_wallpapers": true, "max_wallpaper_count": 50, "wallpaper_path": "C:\Users\Username\Pictures\Wallpapers", "startup_enabled": false }


Plain Text


- 配置修改后会立即生效（部分设置需重启）。
- 开机自启功能会通过系统注册表实现。

## 使用提示

- 画报模式会从指定的壁纸存储目录中随机选择壁纸。
- 空闲检测功能需要系统权限来获取用户输入活动。
- 自动删除功能会保留最近设置的壁纸数量，超出部分会被删除。
- 建议将壁纸存储路径设置为非系统盘，避免占用系统空间。

## 技术栈

- 后端：Python 3
- GUI：PyQt5
- 系统托盘：pystray
- 图像处理：Pillow
- 网络请求：requests（标准库）

## 开源许可证

[MIT](LICENSE)

## 已知限制

- 仅支持 Windows 操作系统。
- 画报模式需要本地有壁纸文件。
- 空闲检测在某些系统配置下可能不准确。

## 贡献

欢迎提交 Issue 和 Pull Request。

---

**若本工具对你有帮助，可以点 ⭐ Star 支持。**
