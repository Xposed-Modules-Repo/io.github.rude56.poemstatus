# 状态栏古诗

在状态栏滚动古诗，或任何你喜欢的文字。

诗句从屏幕右侧滚入、向左滚过状态栏，只遮住诗句正下方那一小段；播完恢复原生时钟，停留片刻后播放下一首。

## 特点

- **完全离线**：不申请 INTERNET 权限，没有任何网络请求
- **静态作用域**：只注入 `com.android.systemui`，不需要也不能勾选其他应用
- **省电**：只在滚动时申请帧回调，静止时零消耗；帧率上限 30fps，位移不足 1px 不重绘
- **双皮肤**：Material 3 与 Miuix（HyperOS 观感）可选，跟随系统深浅色与动态取色

## 功能

- 诗库支持增删改、启停、排序、搜索，纯文本导入导出
- 顺序 / 随机播放，速度 20–600 px/s，停留 0–600 秒
- 作者、出处可单独隐藏
- 横屏、锁屏、指定应用前台时自动暂停
- 可选「洞」：让诗句在指定区域传送（虫洞）或隐藏（隧道）

## 安装

需要 Root 与 LSPosed。

1. 安装 APK
2. 在 LSPosed 中启用本模块（作用域已固定为「系统界面」）
3. 重启系统界面：App → 设置 → 维护 →「重启系统界面」（需 root 授权），或直接重启手机
4. 打开 App，开启总开关

装完或更新模块后必须重启一次系统界面，否则跑的还是旧代码；之后改设置即时生效。

卸载：卸载 APK 后重启系统界面。

## 系统要求

Android 13（API 33）及以上，libxposed API 102。

## 链接

- 源码：https://github.com/Rude56/statusbar-poem
- 问题反馈：https://github.com/Rude56/statusbar-poem/issues

## 许可

[MIT](https://github.com/Rude56/statusbar-poem/blob/main/LICENSE)
