# 本仓库已不再更新，已经整合到：https://github.com/UnrealMultiple/TShockPlugin，后续更新均会发布至此仓库
# This repository is no longer updated and has been integrated into: https://github.com/UnrealMultiple/TShockPlugin. All future updates will be published there.
# ezperm 插件

## 简介

ezperm 插件是一个为 Terraria 服务器设计的 TShock 插件，它提供了一个简化的方式来批量添加或删除玩家组的权限。这个插件特别适合那些需要快速设置或调整服务器权限的管理员。

## 功能

- 通过配置文件定义权限变更，简化权限管理过程。
- 使用 `/inperms` 命令批量执行权限的添加和删除。

## 配置文件

ezperm 插件的配置文件 `ezperm.json` 位于 TShock 的保存路径下。这个 JSON 文件包含了玩家组及其对应的权限变更规则。

配置文件的结构如下：

```json
{
  "Groups": [
    {
      "Name": "组名1",
      "AddPermissions": ["权限1", "权限2", ...],
      "DelPermissions": ["要删除的权限1", "要删除的权限2", ...]
    },
    {
      "Name": "组名2",
      "AddPermissions": ["权限A", "权限B", ...],
      "DelPermissions": ["要删除的权限A", "要删除的权限B", ...]
    }
    // 更多组配置...
  ]
}
```

- **Groups**：一个玩家组配置的数组。
  - **Name**：玩家组的名称。
  - **AddPermissions**：一个字符串数组，包含要添加给该玩家组的权限。
  - **DelPermissions**：一个字符串数组，包含要从该玩家组中删除的权限。

## 使用

在配置文件中设置好玩家组和权限后，管理员可以通过在游戏内输入 `/inperms` 命令来应用这些变更。插件会自动处理配置文件中定义的所有权限变更。

## 开发者信息

- **作者**：大豆子, 肝帝熙恩优化1449

## 支持与反馈

如果您在使用过程中遇到问题或有任何建议，欢迎在官方论坛或社区中提出 issues。

- GitHub 仓库：https://github.com/THEXN/ezprem
