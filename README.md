## [Surveillance Station 9.1.2-10854](https://archive.synology.com/download/Package/SurveillanceStation)
---
### 任务计划
- 控制面板 -> 任务计划  
- 创建 -> 定时任务 -> 用户定义脚本  
- 常规: 用户 = root，取消选中启用  
- 任务设置: 用户定义脚本 = ...  
- 确定 - 确定  
- 单击并运行任务。  
- 在看到有58个许可证时删除此任务。  

---
### A. x86_64 (9.1.2-10854)
- 下载链接: https://global.synologydownload.com/download/Package/spk/SurveillanceStation/9.1.2-10854/SurveillanceStation-x86_64-9.1.2-10854.spk
- 脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/lib/SurveillanceStation-x86_64/install_license)
```

### B. x86_64_openvino (9.1.1-10728)
- 下载链接: https://global.synologydownload.com/download/Package/spk/SurveillanceStation/9.1.1-10728/SurveillanceStation-x86_64-9.1.1-10728_openvino.spk
- 脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/lib/SurveillanceStation-x86_64_openvino/install_license)
```

### C. armada38x (9.0.2-10061)
- 下载链接: https://global.synologydownload.com/download/Package/spk/SurveillanceStation/9.0.2-10061/SurveillanceStation-armada38x-9.0.2-10061.spk
- 脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/lib/SurveillanceStation-armada38x/install_license)
```

---
### 删除许可证&复原
- 脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/lib/license/remove_license)
```
