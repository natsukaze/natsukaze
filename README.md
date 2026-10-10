<h1 align="center">夏風 / natsukaze</h1>

<p align="center">
  <i>路由器固件 · OpenWrt · 嵌入式 C</i>
</p>

<br />

给一块 MediaTek **MT7981B** 的路由器(OpenFi 6C)做固件:内核、设备树,
以及几个直接和硬件打交道的用户态守护进程。

**在做的事**

- 📡 让 OpenFi 6C 完整跑起来 —— 设备树、板级配置、风扇温控、5G 模组、短信收发

- 🧱 底座是 **ImmortalWrt 25.12** + MTK 闭源 WiFi 驱动,维护在自己的 [fork](https://github.com/natsukaze/immortalwrt-mt798x-rebase) 上(上游分支保持纯净,我们的改动单独一条分支)

- 🧪 三个包用 **C** 重写,零外部依赖 —— 配了 800+ 项本地测试、ASan/UBSan、
  模糊测试和变异测试。硬件 I/O 支持注入根目录和 PTY 假设备,
  所以"写 PWM""发 AT"这类以前只能上机试的事,本机就能验证

- 🐛 顺手修了设备树里几处与硬件不符的地方,给上游提了 [PR #111](https://github.com/chasey-dev/immortalwrt-mt798x-rebase/pull/111)
  (模式开关极性、gpio 8 被误当 USB VBUS、SPI-NAND 电气参数、LED 映射)

- 💬 有问题可以直接开 issue

<code><img height="20" alt="c" src="https://raw.githubusercontent.com/github/explore/main/topics/c/c.png"></code>
<code><img height="20" alt="linux" src="https://raw.githubusercontent.com/github/explore/main/topics/linux/linux.png"></code>
<code><img height="20" alt="bash" src="https://raw.githubusercontent.com/github/explore/main/topics/bash/bash.png"></code>
<code><img height="20" alt="shell" src="https://raw.githubusercontent.com/github/explore/main/topics/shell/shell.png"></code>
<code><img height="20" alt="git" src="https://raw.githubusercontent.com/github/explore/main/topics/git/git.png"></code>

| <a href="https://github.com/anuraghazra/github-readme-stats"><img align="center" src="https://github-readme-stats.vercel.app/api?username=natsukaze&show_icons=true&include_all_commits=true&theme=buefy&hide_border=true" alt="natsukaze's github stats" /></a> | <a href="https://github.com/anuraghazra/github-readme-stats"><img align="center" src="https://github-readme-stats.vercel.app/api/top-langs/?username=natsukaze&layout=compact&theme=buefy&hide_border=true" alt="Top Langs" /></a> |
| ------------- | ------------- |

#### 主要仓库

<a href="https://github.com/natsukaze/immortalwrt-mt798x-rebase">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=natsukaze&repo=immortalwrt-mt798x-rebase&theme=buefy" />
</a>
<a href="https://github.com/natsukaze/openfi6c-packages">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=natsukaze&repo=openfi6c-packages&theme=buefy" />
</a>

<br />
<br />
