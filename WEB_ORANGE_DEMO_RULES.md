# WEB_ORANGE_DEMO_RULES

- 规范包路径：`~/.claude/skills/pc-demo-design-guidelines/web端demo规范包`
- 接入日期：2026-08-05
- 目标页面：`index.html`（视觉编译层：`v8-orange.css`，最后加载）

## 硬约束

- 不得改变信息结构、功能逻辑、语义内容、交互行为。
- 内容层背景固定 `#FCFCFC`。
- 任何卡片不得单侧描边、单侧强调线、局部边框。
- 品牌区左上角 logo 使用本包 `assets/logo.svg`（已复制为 `assets/brand/ds-glyph.svg`，置于 `#FF5900` 橙色瓦片）；发起机构展示区使用动势科技官方横版 Logo（用户指定，优先于规范默认）。
- 中间内容区主按钮使用局部辅助蓝紫渐变 `linear-gradient(274deg,#795AFF -12.25%,#5A8CFF 99.85%)`，不使用橙色。
- 表头 `#F9F8FB`；表格/矩阵描边 `#F4F5F7`；无投影、无彩色行底。
- 可见文字不低于 12px。

## 组件映射

| 页面结构 | 标准组件 |
|---|---|
| site-header（brand + desktop-nav + header-apply） | 顶部全局栏 Top Bar |
| hero kv-stage / hero-partner-strip | 页面标题区 + 品牌区 |
| plain-feature-list article | 内容卡片 Card |
| compute-fact | KPI 指标卡片 |
| prize-table | 数据表格 Table |
| scene-matrix | 矩阵表格 Matrix |
| case-flow（tracks）/ case-example / schedule-card / team-mode-card | 内容卡片 Card |
| team-rule | 小信息块（说明条） |
| track-detail / partner-group-head span | Tag / 辅助说明 |
| application-form（input/select/textarea/choice） | 表单 + 筛选框 |
| review-dialog | 弹窗 |
| site-footer | 页脚（应用壳） |

## 未归类组件

- `architecture-scene`（各 section 背景 SVG 蓝图动画）：装饰性背景图形，规范无对应组件类型；暂保留并随 token 换色为橙。需要人工确认归属。
- `kv-field`（品牌 KV 位图）：品牌资产，以 hue-rotate 整体转橙处理。需要人工确认是否更换为橙色版官方 KV。

## 例外记录（用户指令优先）

- 发起机构 Logo：使用动势科技官方橙色横版 lockup（`assets/brand/dongshi-logo.png`），为用户明确指定，符合品牌真实性；规范的 `logo.svg` 用于顶栏/页脚品牌瓦片。
- 页面为营销官网（无侧边栏、无 Agent 面板），按规范"缺省结构规则"不强行新增。
