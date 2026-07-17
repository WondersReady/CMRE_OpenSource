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

## 开源协议

本项目中由 CMRE 贡献者原创并有权授权的源代码、Galaxy 脚本和配置修改采用 [GNU General Public License v3.0](LICENSE) 发布。分发修改版本时，需要遵守 GPL-3.0 并提供相应源代码。

《星际争霸 II》、Blizzard Entertainment 的游戏内容，以及仓库内标明或可识别的第三方模型、贴图、音频和其他素材不因存放在本仓库中而转为 GPL-3.0。相关权利仍归各自权利人所有，详见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。
