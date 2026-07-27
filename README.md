# 足球彩票期望值分析工具

## 项目说明

本仓库包含一个 Reasonix skill，用于分析竞彩足球赔率数据，计算期望值，提供最优投注方案建议。

## 功能

- 竞彩足球赔率数据分析
- 期望值计算
- 最优投注方案推荐
- 多种赔率模型对比

## 依赖

本 skill 需要以下 MCP 服务器配合：

| MCP 服务器 | 用途 | 是否必须 |
|:----------|:----|:--------|
| **Luma MCP** (`mcp__luma-mcp__image_understand`) | 识别赔率截图中的比赛信息和赔率数据 | ✅ 必须 |
| **Firecrawl MCP** (`mcp__firecrawl-mcp__firecrawl_scrape`) | 从专业网站自动采集赔率数据 | ✅ 必须 |
| **web_fetch**（Reasonix 内置） | 补充球队排名、战绩等辅助信息 | ⭐ 推荐 |

**安装方法：**
1. Luma MCP：在 Reasonix 中安装 luma-mcp 插件
2. Firecrawl MCP：在 Reasonix 中安装 firecrawl-mcp 插件
3. 没有以上 MCP 时，用户也可手动输入赔率数据，skill 仍可分析

## 使用方法

### 如果你用 Reasonix

装好 Reasonix 及上述 MCP 后，打开本项目，skill 自动加载。

触发方式：提供竞彩足球赔率截图、比赛ID，或直接粘贴赔率数据。

### 如果你用其他 AI 工具（Claude Code / Cursor / ChatGPT 等）

将 `.reasonix/skills/football-ev/SKILL.md` 的内容作为系统指令提供给 AI，并确保 AI 工具有图像识别和网络搜索能力。

## 许可

MIT
