# AstroBox-NG-Module-App-ESP32C3

针对嵌入式硬件esp32c3的AstroBox-NG客户端

## 编译
以下教程基于macOS Tahoe 26 (aarch64)

先安装：cmake、ninja、dfu-util、ldproxy (走cargo install)

必须使用esp-idf v5.3.3，执行编译时会自动下载，但推荐直接克隆idf仓库然后checkout到5.3.3分支，记得更新submodules，完事直接复制进.embuild/espressif/esp-idf/v5.3.3以加速并节省你的生命

> 注意：该模块依赖独立的交叉编译工具链，已经从 `src-tauri` 顶层 Cargo workspace 中剥离。请直接进入该目录后再运行 Cargo 命令。为了让rust-analyzer正常工作，你通常也需要在编辑器中单独打开该模块的文件夹。
