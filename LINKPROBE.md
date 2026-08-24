# 外链真测 LinkProbe — Remote MCP / 国外网站真实检测

LinkProbe 是一个公开可用的远程 MCP 工具，用服务器真实访问公开 URL，而不是让 AI 猜测网页是否可访问。

**在线使用:** https://linkprobe-qj1j3n.v2.appdeploy.ai/

**Remote MCP Endpoint:** https://linkprobe-qj1j3n.v2.appdeploy.ai/mcp

## 能做什么

- 检测国外链接是否真实返回 HTTP 响应
- 返回 HTTP 状态码和最终 URL
- 跟踪最多 5 次重定向
- 测量响应时间
- 返回 DNS 解析地址
- 检测 HTTPS
- 提取页面标题
- 识别常见访问限制信号：地区限制、验证码、安全挑战、登录墙、付费墙
- 拒绝 localhost、内网 IP 和私有网络目标

## MCP Tool

`check_public_link`

Input:

```json
{"url":"https://example.com"}
```

适合：AI Agent、跨境电商开发者、海外网站测试、链接监控、远程网络排查。

Keywords: MCP, MCP Server, Remote MCP, ModelScope, 魔搭 MCP, 外链检测, 国外网站检测, 网站可用性, HTTP 检测, DNS 检测, 海外链接, AI Agent 工具, 跨境电商工具.
