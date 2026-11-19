# Hi, I'm Du Lei (杜雷)

**高级测试工程师 · AI 质量工程与多端测试架构 | Senior QA Engineer**  
`Beijing, China` · [Personal Site (1dulei.github.io)](https://1dulei.github.io) · [Email](mailto:a1437699690@163.com) · `8+ Years in Multi-Platform & AI QA`

> **务实防漏测 · 低维护自动化 · AI 功能确定性准出。**  
> 8 年多端软件质量保障经验（**51Talk 无忧英语 → 龙湖集团 → 红本科技**），专注于将日常迭代中的高频漏测隐患沉淀为轻量、零冗余的开源测试防线。

---

### Open-Source QA Tools

| Repository | Focus | What Problem It Solves | Verification |
| :--- | :--- | :--- | :--- |
| **[EvalGate](https://github.com/1dulei/evalgate)** | **AI 问答 Agent 与生图准出门禁** | 针对自研教育问答 Agent（「小红小红」）与 AI 生图业务，自动化核查课本知识忠实度（防幻觉）、JSON 卡片结构、少儿不宜生图词拦截、越狱/隐私套取拒止及提示词退化对比（`evalgate diff`）。 | `8/8 准出全绿` · `0 违规逃逸` |
| **[SpecGate](https://github.com/1dulei/specgate)** | **测试左移 PRD 契约与提测风险门禁** | 从需求文档提取带 SHA-256 签名的测试契约，并在提测前精确锚定文件与行号拦截免鉴权遗留、未加锁并发扣减及 Android 离线新进度覆盖等 9 类高危漏洞。 | `4 套基准 1.00 F1` · `零误报` |
| **[TracePilot](https://github.com/1dulei/tracepilot)** | **免定位符浏览器巡检与后台抓包守卫** | 用例不写一行 CSS/XPath 选择器，自动兼容隐藏复选框、div 伪按钮与新弹窗；后台静默拆检全量 `/api/` 响应与本地存储，自动揪出 `payPwd` 哈希外泄与 `HTTP 200 + code:-1` 假成功。 | `内置靶场实跑通过` · `导出截图证据包` |

---

### Core QA Stack

- **AI 功能评测与提效**：问答智能体防幻觉核查 · AI 生图合规审核测试 · 越狱 / Prompt 注入红队测试 · 提示词版本退化对比 · AI 辅助需求盲区拆解
- **多端测试与左移架构**：Android / iOS / 双 Web 后台 / 服务端全链路测试策略 · 复杂状态机与权限边界挖掘 · 提测分支代码风险走读 · 准入准出门禁
- **接口、数据与移动端专项**：RESTful 接口深度测试（越权/幂等） · `Charles / Mitmproxy` 抓包与弱网模拟 · `MySQL` 数据一致性核查 · `Redis` · `Android ADB / Monkey / Crash 定位`
- **自动化巡检与工程底座**：`Python 3.11` · `Playwright` · `Pytest` · 后台被动抓包监听 · `Linux` 日志排查 · `GitHub Actions` CI 集成
