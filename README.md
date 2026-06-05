# fb-checker-dist

账号检测工具 (account_checker_local) 的**自动更新分发仓**。

- `latest.json` — 最新版本清单 (version / url / sha256 / notes)，客户端启动时拉取比对。
- exe 安装包作为各 Release 的**资产 (Assets)** 提供下载。

更新链路：客户端读 `raw .../main/latest.json` → 版本更高则提示 → 一键下载 Release 资产 → 校验 sha256 → 自替换并重启。
