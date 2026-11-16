# BrunoX Runner

**BrunoX Runner** 是一款专为 IntelliJ IDEA 打造的 [Bruno](https://www.usebruno.com/) (`.bru`) API 请求语言支持与运行插件，让你无需离开 IDE 即可完成 `.bru` 接口文件的编写、校验与执行。

---

## 核心功能

* **Bruno 语言支持 (`.bru`)**：
  * 提供自定义词法/语法解析、语法高亮（含 `{{variable}}` 模板变量高亮）与括号匹配。
  * 实时语义与 AST 校验（如重复单例块检查、单文件多 HTTP 方法块检查等）。
  * 上下文智能补全：支持块名称、字典键、枚举值、HTTP Header、断言操作符、注解及环境变量 `{{envVar}}` 补全。
* **单个请求 & 集合运行**：
  * 支持运行单个 `.bru` 文件或递归运行整个目录的 Bruno 请求（基于 Bruno CLI `bru` / `bru.cmd`）。
  * 支持从 **行号槽运行图标 (Gutter)**、**Project 视图右键菜单**、**编辑器右键菜单** 及 **Run Configurations** 启动。
* **双模式 HTTP 执行**：
  * **IDEA 内置 HTTP Client（默认）**：自动转换 `.bru` 请求并在 IntelliJ `Services` 工具窗口中运行。
  * **Bruno CLI 详细报告**：通过 `bru --reporter-json` 执行，并在 `Run` 工具窗口展示完整的请求/响应详情。
* **CLI 自动探测与项目配置**：
  * 自动探测本地 `bru` / `bru.cmd` 路径，可在 **Settings | Tools | Bruno Runner** 中手动指定路径、验证版本，并配置项目级默认环境与常用 CLI 参数。

---

## 兼容性提示

> **与 `Bruno` / `Bruno Language` 插件不兼容：**  
> 本插件注册了独立的 `.bru` 文件类型与语言解析器。与其他 Bruno 插件同时启用会导致文件类型与语法解析冲突，使用前请先禁用或卸载其他同类插件。

---

## 赞赏支持 (Support / Donate)

如果 **BrunoX Runner** 对你的日常开发有所帮助，欢迎请作者喝杯咖啡 ☕：

| 微信赞赏 (WeChat Pay) | 支付宝 (Alipay) |
| :---: | :---: |
| <img src="./wechat.jpg" width="220" alt="WeChat Pay" /> | <img src="./alipay.jpg" width="220" alt="Alipay" /> |

感谢你的支持！
