# linux config
linux 内核相关配置与生成

### 使用方法 <div id="usage-config"></div>
  - 打开 `linux` 内核项目并 `fork` 到自己仓库
  - 克隆已经 `fork` 的内核仓库  `git clone git@github:<用户名>/<内核仓库名>`
  - 进入已 `clone` 的内核仓库根目录，执行 `git remote add linux https://github.com/torvalds/linux.git` 添加上游代码仓库
  - 进入本项目路径执行  `./linux-config -k <你的内核源码根路径>` 即可开始编译最新内核代码

### 常见的使用例子

### 项目中包含的文件
  |项目文件|说明|
  | --- | --- |
  | `config` | linux 的配置文件 |
  | `linux-config` | 项目主要脚本，具体功能下附 |

### 当前项目支持的功能

  - [ ] 更新 `grub` 启动菜单
  - [ ] 安装 `内核文件` 和 `initramfs`
  - [ ] 根据内核文件生成 `initramfs`
  - [ ] 编译生成内核文件和模块文件
  - [x] 同步上游 kernel 代码 <需要按[<sup>1</sup>](#usage-config)完成配置>
