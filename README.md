# Endurance 适配补丁

让《星际穿越》永恒号部件包（[Endurance](https://spacedock.info/mod/1059)，作者 JPLRepo）
贴合当前的模组列表。

全部用 ModuleManager 补丁实现，**不改模组原文件**。

## 只做两件事

**1. 聚变反应堆：发热量归零**

不再需要散热器，也不会因过热停机。
**EC 输出保持原值不动**：每台 3000 EC/s，6 台共 18,000 EC/s。

**2. 维生模块改用现版 USI-LS**

清掉已废弃的 USI 模块名，改用 [USI-LS](https://spacedock.info/mod/1058) 112.x 的 `USILS_*` 体系；
并给医疗舱补上低温休眠（对应它"能让乘员睡眠与唤醒 6 次"的设定）。

## 依赖

- Endurance（本体）
- ModuleManager
- CommunityResourcePack
- USI-LS
- DeepFreeze（可选 —— 只有用到医疗舱低温休眠时才需要）

## 安装

把 `GameData\Endurance_适配` 放进 KSP 的 `GameData` 目录。

## 卸载

删掉 `GameData\Endurance_适配` 整个目录即可。

## 说明

- 本补丁只包含适配 cfg，**不包含 Endurance 本体或 USI-LS 的任何资源**。
- 反应堆发热归零会显著降低这个部件包的难度（不再需要配散热器）。如果你想要原版难度，
  删掉这个目录即可。

## 授权

MIT

---

# Endurance Compat

Compatibility patch that makes the [Endurance](https://spacedock.info/mod/1059) parts pack fit a
USI-based mod list, implemented with ModuleManager: reactor heat production is zeroed (EC output
left untouched), and life support is migrated to the current USI-LS `USILS_*` modules, with
cryo-sleep added to the medical bay.

Requires Endurance, ModuleManager, CommunityResourcePack and USI-LS (DeepFreeze optional).
Licensed MIT. Contains no assets from the original mods.
