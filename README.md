Auto-USTB-GFJY
==========
Auto complete USTB GFJY lessons
北京科技大学国防教育课程自动代理  **` v1.0 `**

<sup> This project only supports Chinese docs. If you are an English user, feel free to contact us. </sup>

-----
> **警告：**
> - 本项目旨在节约同学们的时间，并非进行结业考试作弊。结业考试并不在本项目所支持的范围内。
> - 请避免在国内媒体平台等公共空间传播本项目。


## 介绍 <sub>Intro</sub>
本项目实现了无人值守式地自动完成[北京科技大学国防教育平台](https://gfjy.ustb.edu.cn/)的线上课程任务。

#### 实现的功能
1. **登录：**
   手动输入账号密码后，会显示验证码图片，手动输入验证码后，即可完成登录。
2. **视频课程自动完成：**
   自动获取视频课程列表，并模拟观看视频的操作（每隔若干秒向服务器报告一次播放进度）。
   > **提示：**
   > 1. “观看”是支持多个视频同时进行的。
   > 2. “观看”的过程中并不会播放和下载视频文件，而只是报告播放进度。
3. **课程考试自动完成：**
   自动获取课程考试列表，并模拟考试的操作（在达到一定分数或达到某个最大尝试次数后停止）。
   > **提示：**
   > 1. “考试”不支持多个考试同时进行，且每场考试需要少许时间来提交答案。
   > 2. “考试”的原理是记忆题目和答案，所以程序需要连续几次考试才能达到较高分数，也就是说初次考试会随机作答。

## 使用方法 <sub>Usage</sub>
#### A. 推荐方案
对于 Windows 系统，可前往 [Releases](https://github.com/isHarryh/Auto-USTB-GFJY/releases) 页面，下载 EXE 文件。下载完成后直接运行，然后跟随程序的指引来操作即可。

#### B. 备选方案
对于非 Windows 系统或者开发者，可[下载](https://github.com/isHarryh/Auto-USTB-GFJY/archive/refs/heads/main.zip)（或克隆）本仓库的源码。确保已安装 [Python](https://www.python.org) 3 运行环境，并安装了 Pillow、pycryptodome、requests 库（有条件者建议使用 [Poetry](https://python-poetry.org) 依赖管理工具）。最后，运行 `Main.py` 即可。

## 许可证 <sub>Licensing</sub>
本项目基于 **MIT 开源许可证**，详情参见 [License](https://github.com/isHarryh/Auto-USTB-GFJY/blob/main/LICENSE) 页面。
