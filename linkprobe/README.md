# 外链真测 LinkProbe — 国外网站真实可用性检测 / MCP

**在线使用：** https://linkprobe-qj1j3n.v2.appdeploy.ai/

**MCP Endpoint：** `https://linkprobe-qj1j3n.v2.appdeploy.ai/mcp`

LinkProbe 是一个真实服务器端外链检测工具，不依赖 AI 猜测。它会从服务器实际请求目标网址并返回：

- HTTP 状态码
- 最终跳转地址与跳转链
- 响应时间
- DNS 解析地址
- HTTPS 状态
- 页面标题
- 常见访问限制信号：地区限制、验证码、登录墙、付费墙、Cloudflare challenge、拒绝访问

## 适用场景

- 国外网站检测
- 海外链接检测
- 跨境电商外链检查
- 海外 SaaS / API 可用性检查
- 出海产品页面检查
- 外链跳转检测
- HTTP 状态码检测
- MCP Agent 工具调用
- AI Agent 外部网络能力

## 搜索关键词

国外网站检测、海外网站检测、外链检测、URL 检测、网址可用性、链接跳转检测、HTTP 状态码、海外链接、跨境电商工具、出海工具、MCP、MCP Server、AI Agent 工具、真实网络请求、网站连通性、服务器检测、海外 SaaS 检测。

## MCP

支持 JSON-RPC MCP：

- `initialize`
- `tools/list`
- `tools/call`

工具名：`check_public_link`

### 示例

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "tools/call",
  "params": {
    "name": "check_public_link",
    "arguments": {
      "url": "https://example.com"
    }
  }
}
```

## 安全边界

LinkProbe 拒绝 localhost、私有网络 IP、`.local` / `.internal` 目标，避免被当作开放代理使用。服务只返回检测元数据，不代理目标页面内容。

## Public Beta

当前公开测试版免费开放。正式商业版计划采用按次/批量检测计费。
