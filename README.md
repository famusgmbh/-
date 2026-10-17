# 独立站泳帽定制

本仓库用于独立站泳帽定制项目，当前处于需求与开发准备阶段。

## 当前状态

截至 2026-10-17，本次基础结构整理前：
- 默认分支为 `main`，只有 `README.md`，内容为项目名称的两次重复。
- 共有两次提交：2026-10-15 的 Initial commit，以及 2026-10-17 的 Update README.md。
- 尚无应用代码、依赖清单、运行脚本、测试、部署配置、Issue 或 PR。
- 仓库描述与原 README 只能确认“独立站泳帽定制”；技术栈、平台接入方式及业务规则尚未确认。

本次补充文档与目录骨架，**尚未实现可运行的定制器**。3D 预览、定制内容、订单关联等均需在需求中确认后实施。

## 目录

| 路径 | 用途 |
| --- | --- |
| `docs/requirements.md` | 已知事实、缺失输入与需求确认表 |
| `docs/development.md` | 开发准备、启动状态与后续工程初始化要求 |
| `docs/next-issues.md` | 可直接用于建立 Issue 的优先任务及验收条件 |
| `src/` | 未来应用源码；当前仅说明文件 |
| `assets/` | 模型、图片、字体等素材的接入约定 |
| `tests/` | 未来测试；当前仅说明文件 |
| `.github/ISSUE_TEMPLATE/task.md` | 任务模板 |
| `.github/pull_request_template.md` | PR 模板 |
| `.gitignore` | 本地环境与常见生成文件忽略规则 |

若选定框架或平台要求其他目录，应在工程初始化时调整本骨架。

## 开始开发

需要 Git 和仓库访问权限。先获取文档：

```bash
git clone https://github.com/famusgmbh/-.git famus-cap-customizer
cd famus-cap-customizer
git switch -c feat/confirm-project-scope
```

先填写 [需求确认表](docs/requirements.md)，再按 [开发说明](docs/development.md) 初始化工程。
**当前没有安装依赖或启动应用的命令**，不要执行假定存在的 `npm install` / `npm run dev`。
工程初始化完成后，必须用实际验证过的版本、命令和访问地址更新本说明。

## 下一步

按顺序处理 [Issue 建议](docs/next-issues.md)：
1. 确认项目范围与首版验收标准。
2. 收集素材与印刷规范。
3. 确认技术方案及平台接入方式。
4. 初始化可运行工程与基础检查。
5. 在范围确认后实现首个完整业务流程。

## 协作与配置

- 每项任务使用独立分支，通过 PR 说明变更与验证结果。
- 未确认的要求应记录为待确认，不应由开发者自行视为业务规则。
- 不提交令牌、密码、客户个人信息或真实订单；配置项明确后再增加仅含占位值的 `.env.example`。
- 素材须确认授权和公开范围；本仓库为公开仓库。
- 当前未指定许可证；商业代码及素材的使用授权需另行确认。
