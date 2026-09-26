# 公开免费技能 / 智能体发布渠道清单（调研结果）

> 调研日期：2026-09-26　调研人：WorkBuddy
> 目的：把「图灵数盟 · 数据专家体系」的 52 位专家 + 9 个专家团发布到公开免费的技能市场。
> 署名统一为 **图灵数盟**，网址 https://www.turingtech.net.cn ，邮箱 public@turingtech.net.cn 。

---

## 0. 一句话结论

**几乎所有技能目录都是从「一个公开 GitHub 仓库」自动索引的。**
因此发布链路的第一块基石、也是最高杠杆的一步，是把 61 个技能包推到一个**公开 GitHub 仓库**上。
仓库一旦公开，以下站点会自动收录（无需注册、无需提交）：
SkillsMP、Glama、PulseMCP（自动爬取）、部分 Awesome 列表。
其余站点只需「一个仓库链接 + 一张表单」。

---

## 1. 前置件（已完成 / 待授权）

| 前置件 | 状态 | 位置 |
|---|---|---|
| 61 个标准 `SKILL.md` 技能包 | ✅ 已生成 | `publish-kit/skills/<id>/` |
| 仓库首页 README（52+9 目录表） | ✅ 已生成 | `publish-kit/README.md` |
| 作者署名档案（中英简介三档 + 联系信息） | ✅ 已生成 | `publish-kit/AUTHOR.md` |
| 逐专家发布文案（表单可直接粘贴） | ✅ 已生成 | `publish-kit/skills/<id>/profile.md` |
| 机器可读目录 catalog.json | ✅ 已生成 | `publish-kit/catalog.json` |
| 许可协议 | ⚠️ 暂定 CC BY-NC-ND 4.0，**待您确认** | `publish-kit/LICENSE` |
| 公开 GitHub 仓库 | ⛔ **阻塞点，需您授权** | 待定 |
| 内部路径清洗（去掉 `D:\数盟\...`） | ✅ 已完成 | 全量 61 包 |

---

## 2. Agent Skills 目录 / 市场（核心战场）

| # | 站点 | 网址 | 免费 | 注册/发布方式 | 我能否自动完成 | 备注 |
|---|---|---|---|---|---|---|
| 1 | **Skillstore** | skillstore.io/submit | ✅ | **匿名提交**，仅需填 GitHub 仓库 URL | 🟢 高（可能有人机验证） | 门槛最低，无需账号 |
| 2 | **Agent Skills Directory**（Claude Skills Hub） | claudeskills.info | ✅ | 需**公开 GitHub 仓库**含 `SKILL.md`，再用其提交表单 | 🟡 中（表单 + 审核 24–48h） | 收录 42,000+ 技能，21 类目 |
| 3 | **SkillsMP** | skillsmp.com | ✅ | **自动索引** GitHub 上的 `SKILL.md` | 🟢 高（推仓库后自动） | 自称不审核质量 |
| 4 | **SkillRegistry** | skillregistry.io | ✅ | 必须 **GitHub 账号登录**后上传 | 🔴 需 GitHub 授权 | 有审核，1–2h |
| 5 | **AugmentClaude** | augmentclaude.com | ✅ | 社区市场，有自己的提交流程 | 🟡 中 | 数百技能，有 bundle |
| 6 | **ClaudeSkillsMarket** | claudeskillsmarket.com | ✅ | 独立社区市场，数十技能 | 🟡 中 | 有写技能的教程 |
| 7 | **Anthropic 官方市场** | claude-community 频道 | ✅ | 需打包为 **Claude 插件**后走官方提交流程 | 🔴 需 Claude 账号 + 企业资质 | `claude-plugins-official` 为邀请制，进不去 |
| 8 | **awesome-claude-skills** | github.com/travisvn/awesome-claude-skills | ✅ | Fork → 加条目 → 提 PR | 🟡 中（需 GitHub 账号） | 3–7 天审核 |
| 9 | **agentskills.io** | agentskills.io | ✅ | Agent Skills 开放标准文档站 | — | 不是市场，是规范 |

## 3. MCP 注册表（我们暂无 MCP server，属第二阶段）

> 现状：本项目产出的是 **Skill（知识+流程）**，不是 MCP server（可执行服务）。MCP 注册表要求提供可运行的 `server.json` / 启动命令，**当前不适用**。若后续把「数据产权登记查询」「数据价值诊断」等做成 MCP server，可发以下站点。

| # | 站点 | 网址 | 免费 | 发布方式 | 备注 |
|---|---|---|---|---|---|
| 10 | **官方 MCP Registry** | registry.modelcontextprotocol.io | ✅ | CLI 发布 + 反向域名验证（GitHub/域名） | 根注册表，下游站点都从它同步 |
| 11 | **Glama** | glama.ai/mcp/servers | ✅ | **自动索引** GitHub 仓库 | 收录量最大（3.7 万+） |
| 12 | **Smithery** | smithery.ai | ✅ | GitHub 关联 + `smithery mcp publish` | 提供托管，需账号 |
| 13 | **PulseMCP** | pulsemcp.com | ✅ | 表单提交，**人工精审** | 已暂停提交（2026-09 核实） |
| 14 | **mcp.so** | mcp.so | 部分 | 社区目录，免费档位可提交 | 快速通道收费 $39 |
| 15 | **MCP Market** | mcpmarket.com | ✅ | 表单提交 | 按 GitHub star 排行 |
| 16 | **LobeHub MCP** | lobehub.com/mcp | ✅ | GitHub 链接提交 | 一键安装 |

## 4. 国内智能体平台（分发触达国内用户，但注册门槛高）

| # | 平台 | 网址 | 免费 | 注册方式 | 我能否自动完成 | 备注 |
|---|---|---|---|---|---|---|
| 17 | **扣子 Coze** | coze.cn | 基础版免费 | **手机号 / 抖音账号** | 🔴 需您本人手机验证 | 可发布到微信、抖音分发 |
| 18 | **腾讯元器** | yuanqi.tencent.com | 基础版免费 | **微信 / QQ 登录** | 🔴 需您扫码 | 无缝接入公众号、小程序 |
| 19 | **文心智能体平台** | agents.baidu.com | ✅ | **百度账号 + 手机号** | 🔴 需手机验证 | 可分发到百度搜索 |
| 20 | **智谱清言智能体** | chatglm.cn | ✅ | 手机号 | 🔴 需手机验证 | 零代码创建 |
| 21 | **ModelScope 魔搭** | modelscope.cn | ✅ | 阿里账号（邮箱可注册，通常需手机） | 🟡 部分可试 | 有 MCP 广场 + 创空间 |
| 22 | **阿里云百炼** | bailian.console.aliyun.com | 有免费额度 | 阿里云账号（实名） | 🔴 需实名 | 企业向 |
| 23 | **讯飞星辰 Agent** | xinghuo.xfyun.cn | 有免费额度 | 手机号 + 实名 | 🔴 需实名 | 企业向 |
| 24 | **Dify** | dify.ai | ✅ 开源 | 邮箱注册 / 自部署 | 🟡 中 | 有插件市场，走 GitHub 提交 |
| 25 | **Gitee（码云）** | gitee.com | ✅ | 邮箱/手机号 + 验证码 | 🔴 有图形验证码 | 国内 GitHub 替代，可镜像仓库 |

## 5. 通用 AI 目录 / 媒体（可选，做品牌曝光）

| # | 站点 | 网址 | 说明 |
|---|---|---|---|
| 26 | Hugging Face Hub | huggingface.co | 可托管数据集/模型/Spaces；邮箱注册有验证码 |
| 27 | Product Hunt | producthunt.com | 发布产品，需账号，适合做单次曝光 |
| 28 | 掘金 / CSDN / 知乎 | — | 发技术长文，把专家包作为配套资源引流 |

---

## 6. 现实约束（必须让您知道的）

1. **人机验证（CAPTCHA）**——GitHub、Gitee、Hugging Face、以及多数表单站点都有滑块的图形验证码。**我无法代替您通过验证码**，遇到时会停下来请您在浏览器点一下。
2. **手机号 / 实名**——国内平台（扣子、元器、文心、智谱、百炼、讯飞）全部要求手机验证或实名认证，**必须由您本人操作一次**。我能做的是把简介、标签、人设文本全部写好，您扫码后粘贴。
3. **GitHub 授权是总闸门**——第 2、3 节里几乎每个站点都要 GitHub 账号。要么您给我一个 Personal Access Token（我只用来建仓库和推代码），要么您授权我用本机已登录的 GitHub 走浏览器自动化。
4. **内容公开授权**——52 位专家 + 9 个专家团的**全部知识底座**将公开在互联网上（含政策文号、SOP、交付物清单、话术）。您们自己的 `10-RESEARCH-AND-OPEN-QUESTIONS.md` 里也把「52 位专家是否全部对互联网公开」列为**上线前必须回答**的问题。请确认。
5. **许可协议**——暂定 CC BY-NC-ND 4.0（署名、非商用、禁演绎）。若要允许商用/二次开发，请指定。

---

## 7. 建议执行顺序

| 阶段 | 动作 | 需要谁 |
|---|---|---|
| **P0** | 推公开 GitHub 仓库 `turing-data-experts`（61 包 + README + catalog） | 需您给 GitHub 授权 |
| **P1** | 提交 skillstore.io（匿名表单，1 次） | 我可自动 |
| **P2** | 提交 claudeskills.info + AugmentClaude + ClaudeSkillsMarket | 半自动，遇验证码暂停 |
| **P3** | SkillRegistry（GitHub 登录） | 需 GitHub 授权 |
| **P4** | 国内平台（扣子 / 元器 / 文心）——我备好文案，您扫码发布 | 您操作 + 我供文案 |
| **P5** | 把「数据产权登记查询」「数据价值诊断」做成 MCP server，再发 MCP 注册表 | 后续开发 |
