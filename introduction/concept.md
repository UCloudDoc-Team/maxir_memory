# 产品概述

## 什么是 MAXIR Memory

MAXIR Memory 是UCloud 平台推出的企业级 AI 记忆与知识管理服务。自动从对话中提炼结构化记忆，跨会话持久存储与精准召回，让 AI 真正拥有长期记忆；支持企业文档知识库管理，通过 MCP 协议及 OpenClaw 插件无缝接入 Claude、Cursor、OpenClaw 等主流 AI 工具和 AI 智能体。

## 核心概念

### 项目（Project）

项目是 MAXIR Memory 的核心组织单元，将相关文档、记忆和 MCP 配置归组管理。每个项目：

- 关联多个文档和文件夹（来自个人云盘或外部连接器）
- 包含多条文字记忆（知识片段和使用说明）
- 提供独立的 MCP 端点和 API Key，供外部 AI 访问


### 文档管理（Document Management）

MAXIR Memory 提供云端文档管理能力：

- 支持上传 PDF、Word、Excel、CSV、Markdown、TXT 等格式
- 层级文件夹组织，支持注释
- 关联到项目后建立索引，AI 可通过 MCP 协议检索文档内容

### 连接器（Connector）

通过 OAuth 认证接入外部文档服务，无需手动下载和重新上传，即可在 MAXIR Memory 中浏览和使用外部文档并与项目关联。WPS（金山文档）、Dropbox、飞书等连接器即将推出。

### MCP 服务器

每个项目可以生成独立的 MCP（Model Context Protocol）端点和 API Key。通过 MCP，支持 MCP 协议的 AI 工具（如 Claude Desktop）可安全访问项目文档和记忆。

## 适用场景

| 场景 | 描述 |
|------|------|
| AI 助手长期记忆 | 通过 API 将对话提交到项目，AI 在后续对话中可检索历史记忆 |
| 企业知识库 | 上传企业文档，通过 MCP 让 AI 工具安全检索知识内容 |
| 研究资料管理 | 管理论文和研究笔记，接入 AI 辅助检索和分析 |
| AI Agent 上下文 | 为 Agent 提供持久化项目知识，支持多轮任务执行 |
