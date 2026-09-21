# GZH888 · 公众号草稿同步 MCP

把文章草稿**原样**同步到微信公众号草稿箱的标准 MCP 服务（试用版）。

- 产品介绍与接入指南：<https://01men.github.io/GZH888/>
- 在线试用（网页直接发草稿）：<https://01men.github.io/GZH888/try.html>
- MCP 端点：`https://atest-0gvlenb46567649d.service.tcloudbase.com/wxdraft/mcp/`

## 三步接入

1. 公众号后台「设置与开发 → 基本配置 → API IP 白名单」加入 `101.34.223.206`
2. 把 MCP 地址配置到你的 AI 客户端（Claude / Cursor / Cherry Studio…）：

```json
{
  "mcpServers": {
    "gzh-draft": {
      "url": "https://atest-0gvlenb46567649d.service.tcloudbase.com/wxdraft/mcp/"
    }
  }
}
```

3. 对 AI 说一句话，发一篇草稿。

## 目录

| 文件 | 说明 |
| --- | --- |
| index.html | 产品介绍页（GitHub Pages 首页） |
| try.html | 网页一键试用 |
| assets/ | 配置指引截图 |

## 能力

- 原样保真：正文只替换图片地址，样式/文本/结构零改动
- 图片自动入公众号素材库，杜绝外链裂图
- 多公众号记忆：首次提供 AppID/Secret，之后只需 AppID
- 图片格式 png/jpg/gif/bmp，单张 ≤10MB，一次 ≤8 篇

试用或商务合作：961589511@qq.com
