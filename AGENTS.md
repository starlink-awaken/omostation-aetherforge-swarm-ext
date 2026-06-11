# AGENTS.md — AetherForge Swarm Extensions

> eCOS v5 蜂群扩展模块 · ILS 搜索 + Perception 感知 + Planning 规划 + Legacy 桥接

## Quick Commands

```bash
cd projects/aetherforge-swarm-ext
uv run pytest tests/ -q
uv run ruff check src/
```

## Architecture

扩展层补充 AetherForge 核心引擎的能力：

```
aetherforge/              ── 核心引擎
aetherforge-swarm-ext/    ── 扩展模块（本仓）
swarm-engine/             ── 群体智能调度
```

### 模块

| 模块 | 职责 |
|:-----|:------|
| `ils/` | 智能体搜索与发现 |
| `perception/` | 环境感知与状态收集 |
| `planning/` | 任务规划与分解 |
| `legacy/` | 兼容层与迁移桥接 |

## Dependencies

- Python >=3.10, uv
- 依赖 aetherforge 核心 SDK

## Testing

```bash
uv run pytest tests/ -q
```
