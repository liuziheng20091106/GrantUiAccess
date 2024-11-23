# UIAccess 提权

> 提权方法及核心由 Doubx690i(Dubi906w/kriastans) 提供。

本插件可以为 ClassIsland 提升 UIAccess 令牌，使 ClassIsland 可以置顶到全屏 UWP 应用和系统界面上。

> [!caution]
> **注意事项：**
>
> - 您需要[以管理员身份运行 ClassIsland ](#使用方法)才能正常使用本插件的功能。
> 
> - 本插件进行的操作涉及敏感操作，可能会触发安全软件拦截。建议将 ClassIsland 工作目录添加到安全软件的排除名单中，以避免误报。

## 截图

![图片](https://github.com/user-attachments/assets/8dcd9bc7-7b60-4584-be39-a9843d9a3c97)


## 使用方法

1. 在插件市场下载并安装插件
2. 下载并安装自动提权插件[CIUACHelper(可在插件市场找到)](https://github.com/liuziheng20091106/CIUACHelper)。（感谢 liuziheng20091106 提供插件）
   >你也可以使用[旧方法](#旧方法)来设置管理员提权，这可以确保你的 Classisland 能够被传入参数。
4. 启动 ClassIsland，如果一切没有问题，插件会自动为应用提升 UIAccess。

### 旧方法
1. 在运行时提权：在 ClassIsland 应用文件属性 -> 【兼容性】页面中勾选【以管理员身份运行此程序】，以在运行 ClassIsland 时自动以管理员身份运行。
   > 仅进行此操作会导致【应用设置】 -> 【常规】 -> 【开机自启】功能失效。
2. 修复开机自启：安装插件[StartUpAsAdmin(可在插件市场找到)](https://github.com/ClassIsland/StartUpAsAdmin)，并按照其中的方法设置计划任务启动
   > 你需要同时设置 在运行时提权 来保证你的每一次启动都是管理员身份运行。

## 致谢

提权方法及核心由 Doubx690i(Dubi906w/kriastans) 提供。

本项目使用了以下第三方库：

- [uiaccess](https://github.com/killtimer0/uiaccess/tree/master/uiaccess)
- [ClassIsland.PluginSdk](https://github.com/ClassIsland/ClassIsland)

## 许可证

本项目基于 [GNU General Public License v3.0](https://github.com/HelloWRC/GrantUiAccess/blob/master/LICENSE.txt) 许可。
