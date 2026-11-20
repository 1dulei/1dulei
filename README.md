# Hi, I'm Du Lei (杜雷)

**高级测试工程师 · AI 质量工程与多端测试架构 | Senior QA Engineer**  
`Beijing, China` · [Personal Site (1dulei.github.io)](https://1dulei.github.io) · [Email](mailto:a1437699690@163.com) · `8+ Years in Multi-Platform QA`

> **务实防漏测 · 低维护巡检 · 明确边界与局限。**  
> 8 年多端软件质量保障经验（**51Talk 无忧英语 → 龙湖集团 → 红本科技**）。以下三个仓库均基于日常测试痛点脱敏后独立实现的个人开源工具，不含任何公司代码或数据。

---

### Personal Open-Source QA Tools

| Repository | Focus | What Problem It Solves | Status & Verification |
| :--- | :--- | :--- | :--- |
| **[EvalGate](https://github.com/1dulei/evalgate)** | **大模型功能上线评测与红队检查** | 面向教育问答助手与 AI 生图等场景（脱敏示例），提供确定性断言、可选 `llm_judge` 逻辑矛盾复核、按「泄露优先于拒绝」顺序判定的红队检查与版本对比（`evalgate diff`）。 | `11 项单测（含 6 条自查 bug 回归）` · 含设计取舍与已知局限 |
| **[SpecGate](https://github.com/1dulei/specgate)** | **提测前 PRD 契约与 Diff 风险检查** | 从需求文档提取带 SHA-256 摘要的非可执行测试契约；11 条规则同时检查 diff 新增行与删除行（含删除权限/事务注解、多行空 catch、离线覆盖等），每条带 `file:line`。 | `10 例评测（4 种子全过 / 6 难例 3 过）` · 盲区透明记录 |
| **[TracePilot](https://github.com/1dulei/tracepilot)** | **浏览器流程巡检 + 后台被动接口检查** | 用例只写可见业务文字，采用「语义定位优先 + 组件兼容降级」并接管 `window.open` 新页签；后台被动检查敏感字段泄露、`localStorage` 明文密码与 HTTP 200 假成功（可配置）。 | `7 项测试（5 守卫单测 + E2E + 契约衔接）` · 输出截图证据报告 |

---

### Core QA Stack

- **AI 功能测试与提效**：问答助手准确性与合规验收 · AI 生图敏感词过滤测试 · 提示词退化对比 · AI 辅助需求盲区拆解
- **多端测试与左移**：Android 学习平板 / App / 双 Web 后台 / 服务端全链路测试策略 · 状态机与权限边界挖掘 · 提测分支变更风险走读 · 准入准出门禁
- **接口、数据与移动端专项**：RESTful 接口测试（越权/幂等） · `Charles / Mitmproxy` 抓包与弱网模拟 · `MySQL` 数据一致性核查 · `Redis` · `Android ADB / Monkey / Crash 定位`
- **自动化巡检与工具**：`Python 3.11` · `Playwright` · `Pytest` · 后台被动接口检查 · `Linux` 日志排查 · `GitHub Actions` CI 集成
