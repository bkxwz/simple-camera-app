# Simple Camera

一个极简的安卓相机应用，专注于快速拍照。

## 功能
- 打开即用，启动速度快
- 单按钮设计，底部中央拍摄键
- 拍照后震动反馈
- 照片保存到设备相册的 "SimpleCamera" 文件夹

## 技术栈
- 原生Kotlin开发
- CameraX相机API
- 最低支持Android 7.0 (API 24)

## 构建
本项目使用GitHub Actions自动构建。

### 手动构建
1. 克隆仓库
2. 使用Android Studio打开项目
3. 构建项目

### 自动构建
每次推送到main分支时，GitHub Actions会自动构建debug APK并上传到Artifact。

## 版本发布
1. 更新`app/build.gradle`中的版本号
2. 创建git tag: `git tag v0.1.0`
3. 推送tag: `git push origin v0.1.0`
4. GitHub Actions会自动创建Release并上传APK

## 安装
1. 从GitHub Releases下载最新APK
2. 在Android设备上启用"未知来源"安装
3. 安装APK

## 权限
- 相机权限：用于拍照
- 存储权限（Android 9及以下）：用于保存照片

## 项目结构
```
simple-camera-app/
├── app/
│   ├── src/main/
│   │   ├── java/com/example/simplecamera/
│   │   │   └── MainActivity.kt
│   │   ├── res/
│   │   │   ├── layout/activity_main.xml
│   │   │   └── values/
│   │   └── AndroidManifest.xml
│   └── build.gradle
├── .github/workflows/build.yml
└── README.md
```

## 许可证
MIT License
