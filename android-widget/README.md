# 单向历安卓桌面小组件

适配 Android / 小米 HyperOS 的原生桌面小组件。默认从以下地址获取当天图片：

`https://img.owspace.com/Public/uploads/Download/YYYY/MMDD.jpg`

日期固定使用 **Asia/Shanghai（北京时间）**。小组件在每天北京时间 00:05 左右安排更新，点击图片可立即重试；图片会缓存在应用私有目录，网络失败时保留上一次成功图片。

## 安装

构建完成后，从本仓库的 **Releases** 下载 `SingleCalendarWidget.apk`，在手机上安装。首次安装可能需要允许当前来源安装应用。

安装后，长按桌面空白处 → 小组件 → 找到「单向历」→ 添加。建议选择较大的竖向尺寸以便完整查看原图。

## 构建

需要 JDK 17、Android SDK Platform 35 和 Gradle 8.9：

```sh
cd android-widget
gradle assembleDebug
```

APK 输出位置：`app/build/outputs/apk/debug/app-debug.apk`。

## 隐私

应用仅请求联网和开机后恢复日历更新所需的权限；没有账号、广告、分析 SDK 或应用内跟踪。
