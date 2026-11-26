# 阿里云飞天企业版（专有云）中文文档 — Markdown 版

本仓库收录整理后的 **Alibaba Cloud Apsara Stack（阿里云专有云 / 飞天企业版）** 中文产品文档 Markdown 转换版，按版本、11 个产品大类与产品 code 归档。

## 版本与规模

| 目录 | 说明 | 文档数 | 页数 |
| :--- | :--- | :---: | :---: |
| `v_3_18_6_20250430/` | V3.18.6（20250430 版） | 269 | — |
| `v_3_18_6_20260730/` | v3.18.6-SP2607（20260730 版） | 288 | — |
| `v_3_18_6_20261030/` | v3.18.6（20261030 版） | 231 | — |
| `legacy/` | 3.18.6 前保留的独有文档（`eip`、`terraform`、`asr`） | 10 | — |
| **合计** | `798` 份文档 / `11` 个产品大类 / `49` 个 3.18.6 产品 + `2` 个 legacy 产品 | **798** | **126,059** |

## 目录大类（11 类）

`云平台`、`计算`、`存储`、`网络`、`数据库`、`中间件`、`大数据`、`安全`、`监控与运维服务`、`容灾与迁移`、`OpenTrek`

## 说明

- **图片资源**：每篇文档配有同级独立 `<assets_dir>/` 目录（如 `zh-api-gateway-user-guide-v3.18.6-20260528.assets/`），互不共用，便于单独维护；图片已保留原分辨率并按 WebP `q=90`（体积未变小时保留原 PNG）压缩，仓库总检出体积约 `1.34 GiB`。
- **原版 PDF 下载**：完整未修改的原版 PDF 分版本打包保存在本仓库的 [Releases (`pdf-v3.18.6`)](https://github.com/lancenty/apsara-docs-zh/releases/tag/pdf-v3.18.6)。
- **校验清单**：根目录 [`manifest.json`](manifest.json) 记录每份文档的 `document_id`、SHA256、页数与资源清单，已全部通过渲染与链接一致性校验（`0` 错误、`0` 冲突）。

## 文档 ID

`manifest.json` 中每份文档的 `document_id` 分六段，与发布包目录一一对应：

```
{language}/{package_version}/{category}/{product_code}/{document_key}/{document_version}
```

例如 `OpenTrek/opentrek/` 下的“智能体工厂 OpenTrek AI Gateway 产品简介 20260528.pdf”（属于 20250430 发布包）：

```
zh-cn/3.18.6_20250430/opentrek/opentrek/ai-gateway-product-introduction/20260528
```

| 段 | 含义 | 示例 |
| :--- | :--- | :--- |
| `language` | 语言 | `zh-cn` |
| `package_version` | 发布包版本 + 发布日期 | `3.18.6_20250430`、`legacy` |
| `category` | 一级分类 slug | `opentrek`、`compute`、`security` |
| `product_code` | 产品代码 | `opentrek`、`ecs`、`aegis` |
| `document_key` | 文档主题（同一产品代码下多产品时带产品前缀） | `ai-gateway-product-introduction` |
| `document_version` | 文档版本（封面八位日期） | `20260528` |

