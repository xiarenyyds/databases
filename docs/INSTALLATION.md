# 数据库下载与使用

打开 MDCx，对应页面点击“下载”，确认下载网址后点击“下载并替换”。

| 页面 | 下载文件 |
| --- | --- |
| Amazon ASIN | `amazon-asin.sqlite3` |
| 演员资料 | `actor-profile.sqlite3` |
| 演员映射／信息映射 | `actor-mapping.sqlite3` |

三个文件分别存储资料；演员与信息映射保存在同一个文件的不同表中。首次启动创建空库，不会自动联网下载。

已有客户端尚未预填网址时，从 [仓库首页](../README.md) 复制对应文件的下载链接填入。链接始终指向最新正式版本。

主程序下载时校验类型、结构版本、字段、索引和完整性。下载成功后完整替换对应数据库，本地维护结果也会被替换；失败保留原库。

手动下载的用户可同时获取 `SHA256SUMS.txt` 核对文件是否完整。Linux 使用 `sha256sum -c SHA256SUMS.txt`，macOS 使用 `shasum -a 256 -c SHA256SUMS.txt`，Windows 使用 PowerShell 的 `Get-FileHash` 与清单对照。

说明与更新日志保存在仓库，发布附件仅包含三个 SQLite 文件与校验清单。
