# EEBBK S10 / volcano — TWRP 公开骨架

此仓库属于 **EEBBK BOOM**，仅用于展示 EEBBK S10（设备代号 `volcano`）的 TWRP 项目及目录结构。

**这是刻意裁剪的不完整设备树，不具备编译能力，也不提供可刷写镜像。**

## 设备公开规格

| 项目 | S10 规格 |
| --- | --- |
| 品牌 / 型号 | 步步高（EEBBK）S10 学习机 |
| 移动平台 | **Qualcomm Snapdragon 6 Gen 4** |
| 芯片型号 | **SM6650（本机原厂标识 SM6650P）** |
| CPU / 制程 | 8 核 Kryo CPU，4 nm 制程，平台最高约 2.3 GHz |
| GPU / AI | Qualcomm Adreno GPU、Qualcomm AI Engine（平台特性） |
| 屏幕 | 14.2 英寸类朗伯光刻护眼屏，2328 × 1600，120 Hz |
| 内存 / 存储 | 8 GB RAM + 256 GB |
| 无线连接 | Wi-Fi 6（2×2 MIMO）、蓝牙 5.0 |
| 电池 / 充电 | 10000 mAh 典型容量，支持 30 W 充电 |
| 接口 | USB Type-C |
| 手写笔 | 磁吸充电手写笔 |

高通平台资料：[Snapdragon 6 Gen 4 Mobile Platform](https://www.qualcomm.com/smartphones/products/6-series/snapdragon-6-gen-4-mobile-platform)。
设备标识来自原厂设备树和内核证据；S10 官网参数来自[步步高 S10 官方产品页](https://www.eebbk.com/html/pc/products/s10.html)（2026-11-22 查阅）。平台最高规格不代表 S10 已启用每项可选功能，也不把 Snapdragon 平台的蜂窝、显示或摄像头能力当作本机配置。

## 公开内容

- 设备名称及代号。
- 设备树预编译资源目录的空占位文件。
- 本仓库的内容范围说明。

## 未公开内容

以下内容没有包含在本仓库中：

- `BoardConfig.mk`、`device.mk`、`AndroidProducts.mk`、产品 makefile 等核心构建配置。
- `recovery.fstab`、init/USB/安全服务配置和硬件适配参数。
- TWRP 源码补丁及其他修改实现。
- 构建、打包、提取、签名脚本及源码固定版本清单。
- 内核、DTB、驱动模块、字体、主题素材等预编译文件。
- 签名密钥、认证信息、设备日志和个人数据。

目录中的 `.gitkeep` 仅用于保留空目录，不代表相应实现已经公开。

## 目录

```text
.
├── README.md
├── docs/
│   └── DEVICE.md
└── prebuilt/
    ├── config/       # 空占位
    ├── dtb/          # 空占位
    ├── recovery/     # 空占位
    ├── theme/        # 空占位
    └── vendor_boot/  # 空占位
```

不要尝试使用本仓库直接构建或刷写设备。
