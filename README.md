# MDCx 数据库

本仓库单独发布 MDCx 使用的数据库，文件与 SHA-256 校验清单放在 [最新版本](https://github.com/xiarenyyds/databases/releases/latest) 中。

| 数据库 | 文件 | 下载 |
| --- | --- | --- |
| Amazon ASIN 对照库 | `amazon-asin.sqlite3` | [下载](https://github.com/xiarenyyds/databases/releases/latest/download/amazon-asin.sqlite3) |
| 演员资料库 | `actor-profile.sqlite3` | [下载](https://github.com/xiarenyyds/databases/releases/latest/download/actor-profile.sqlite3) |
| 演员、信息映射共用库 | `actor-mapping.sqlite3` | [下载](https://github.com/xiarenyyds/databases/releases/latest/download/actor-mapping.sqlite3) |

在 MDCx 对应数据库页面点击“下载”。默认网址指向本仓库，也可将上面的下载链接填入已有客户端的下载输入框。

下载完成后，主程序校验数据库类型、结构和完整性，通过后完整替换对应本地数据库；本地新增、修改与删除的结果也会被替换。下载或校验失败保留原库。

[使用说明](docs/INSTALLATION.md) · [更新日志](CHANGELOG.md)

主程序安装包：[MDCx-Rust](https://github.com/xiarenyyds/MDCx-Rust)；Emby 插件：[MediaAssistant](https://github.com/xiarenyyds/MediaAssistant)。
