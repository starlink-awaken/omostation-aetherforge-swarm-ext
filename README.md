# AetherForge Swarm Extensions

> AetherForge 蜂群扩展模块 — ILS 智能体搜索、Perception 感知、Planning 规划、Legacy 兼容层。

## 层位置

eCOS v5 蜂群基础设施的扩展面：

```
projects/aetherforge/      ── 核心蜂群引擎
projects/aetherforge-swarm-ext/ ── 扩展模块（本仓）
projects/swarm-engine/     ── 群体智能调度
```

## 包

| 模块 | 职责 |
|:-----|:------|
| `ils` | 智能体搜索与发现 |
| `perception` | 环境感知与状态收集 |
| `planning` | 任务规划与分解 |
| `legacy` | 兼容层与迁移桥接 |

## Quick Start

```bash
uv sync
uv run pytest tests/ -q
```

## 依赖

- Python >=3.10
- uv 包管理器
