# OA Purchase Request

Frappe app for creating and maintaining the custom `OA Purchase Request` DocType in ERPNext.

## 协作入口

OA 采购申请及审批接入的独立仓库为 [yueweiit/deeplinkerp-oa_purchase_request](https://github.com/yueweiit/deeplinkerp-oa_purchase_request)，从 `main` 分支更新后开发，PR 目标也选择 `main`，Frappe App 名保持 `oa_purchase_request`。
2026-10-16 的应用基线与线上 `cecb3b2c9e3c48217dbe127327ea8f2d5ee40ea7` 完全一致，生产源码标签为 `production/2026-10-16/oa_purchase_request`。
整理前的主线保存在合并历史；上述生产标签及 `archive/2026-10-16/oa_purchase_request-before-production-alignment` 标签继续保留于原仓库 `yueweiit/DeepLinkERP`；原先仅在本地保存的生产提交已归档到 GitHub。
跨应用修改拆分相应 PR 并说明依赖，详见[独立仓库说明](https://github.com/yueweiit/deeplinkerp-deeplinkerp_branding/blob/main/docs/contributing/erp-branches.md)。
本次没有部署服务器、运行 DocType 初始化或修改业务数据；发布仍使用现有流程。

Install on a site:

```bash
bench --site dev.localhost install-app oa_purchase_request
```

Run the DocType setup manually:

```bash
bench --site dev.localhost execute oa_purchase_request.install.create_or_update_oa_purchase_request
```
