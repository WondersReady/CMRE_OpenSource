# CMRE OpenSource

CMRE 的核心 Mod、启动/测试地图，以及 `CM_EMaps` 地图集合。

## 项目内容

核心 Mod 位于 `Mods/CMRE`：

- `CMRE_Core_Base.SC2Mod`
- `CMRE_Core_Mengsk.SC2Mod`
- `CMRE_Core_Stetmann.SC2Mod`
- `CMRE_Core_Triggers.SC2Mod`

启动和测试地图位于 `Maps/CMRE`：

- `Launcher.SC2Map`
- `TestMap.SC2Map`

额外地图位于 `Maps/CM_EMaps`。

## 安装路径

将仓库根目录中的 `Mods` 和 `Maps` 文件夹复制到《星际争霸 II》根目录，并与已有同名文件夹合并。

安装后的目录结构必须如下：

```text
<StarCraft II>
|-- Mods
|   `-- CMRE
|       |-- CMRE_Core_Base.SC2Mod
|       |-- CMRE_Core_Mengsk.SC2Mod
|       |-- CMRE_Core_Stetmann.SC2Mod
|       `-- CMRE_Core_Triggers.SC2Mod
`-- Maps
    |-- CMRE
    |   |-- Launcher.SC2Map
    |   `-- TestMap.SC2Map
    `-- CM_EMaps
        `-- *.SC2Map
```

`<StarCraft II>` 是游戏安装根目录，例如：

```text
D:\Game\StarCraft II
```

Mod 的 `Mods\CMRE` 路径不能改名，否则本地文件依赖将无法解析。地图可以放在 `Maps` 下，但建议保持上面的 `Maps\CMRE` 和 `Maps\CM_EMaps` 结构。

## 外部依赖

本仓库不包含以下依赖：

- `Mods\CM_ArtPack\CM_ArtPack_Base.SC2Mod`：由 `CMRE_Core_Base.SC2Mod` 引用。
- `Mods\CM\CM_Core_Extra.SC2Mod`：由 `Maps\CM_EMaps` 中的地图引用。

编辑器能够使用对应的战网依赖时，可以直接解析；需要完全本地运行时，请另外安装这些依赖并保持上述路径。

## 扩展内容

作者包、整合包、突变因子包和威望包位于独立项目 `CMRE_Extensions`。安装扩展前应先安装本项目。

## 来源与致谢

CMRE 使用的原始基础代码与数据来自 Blizzard Entertainment（暴雪娱乐）官方《星际争霸 II》内容。项目初期以 Maguro 开发的 MM 系列合作地图作为开发模板，CMRE 贡献者在此基础上进行了后续修改、扩展与整合。

感谢 Blizzard Entertainment 提供原始游戏内容，也感谢 Maguro 对《星际争霸 II》合作模式地图开发与社区创作所作的贡献。上述来源与致谢不表示 Blizzard Entertainment 或 Maguro 对 CMRE 的认可、赞助或背书。

## 开源协议

本仓库及其内容的使用、开发与分发首先受适用的 [Blizzard End User License Agreement（EULA）](https://www.blizzard.com/en-us/legal/fba4d00f-c7e4-4883-b8b9-1b4500a402ea/blizzard-end-user-license-agreement) 和 [Custom Game Acceptable Use Policy](https://www.blizzard.com/en-us/legal/2749df07-2b53-4990-b75e-a7cb3610318b/custom-game-acceptable-use-policy) 约束。暴雪的自定义游戏政策明确纳入 EULA，并规定两者冲突时以自定义游戏政策为准。

[GNU General Public License v3.0](LICENSE) 及仓库中的其它许可声明，仅适用于未被上述暴雪条款覆盖、可以与相关游戏内容分离、且 CMRE 贡献者确实有权授权的原创部分。GPL-3.0 不对《星际争霸 II》、Custom Game、Blizzard Entertainment 的游戏内容或第三方材料作任何重新授权；如许可条款发生冲突，暴雪条款对其覆盖的内容优先适用。

仓库内标明或可识别的第三方模型、贴图、音频和其他素材仍受各自权利人的条款约束，详见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。本节只是适用范围说明，不能替代暴雪官方条款或法律意见。
