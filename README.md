# [Surveillance Station 9.2.0-11289](https://archive.synology.com/download/Package/SurveillanceStation)

---
[尊重版权，此仓库仅做搬运和国内加速，请点击我阅读原作者的所有信息！](https://github.com/ohyeah521/Surveillance-Station)
---

---
### 任务计划
> ⚠️如果你会使用SSH则不需要看这部分
- 控制面板 -> 任务计划  
- 创建 -> 定时任务 -> 用户定义脚本  
- 常规: 用户 = root，取消选中启用  
- 任务设置: 用户定义脚本 = ...  
- 确定 - 确定  
- 单击并运行任务。  
- 在看到有60个许可证时删除此任务。  


### 免责声明

🥤本研究旨在为了学术和技术交流的目的，探讨商业软件注册限制的绕过方法。

**特别声明：**

1. 本研究仅用于学术研究和技术学习，不得用于任何违法或不正当的目的，包括但不限于商业用途、侵权行为或破坏性操作。
2. 研究成果的发布不代表对绕过方法的推广或鼓励，也不对任何由此产生的法律责任或后果承担责任。
3. 用户应自行确保在进行任何相关操作之前，已经获得软件供应商的授权许可，并遵守所有相关法律法规。
4. 本免责声明不适用于任何违反法律法规的行为，作者不对因使用本研究成果而产生的任何法律责任、经济损失或其他不良后果承担责任。

请使用者在使用本研究成果时，自觉遵守法律法规，并对自己的行为负责。

---
## ⚠️⚠️⚠️注意
若遇到最新版群晖系统提示“11289与您的Synology NAS不兼容，请上传9.2.1-11320或以上版本”导致无法安装，请执行以下代码，通过SSH或者计划任务执行均可：
```
cp /etc.defaults/synopackageslimit.conf /etc.defaults/synopackageslimit.conf.bak
sed -i 's/SurveillanceStation="9.2.1-11320"/SurveillanceStation="9.2.0-11289"/g' /etc.defaults/synopackageslimit.conf
```

若后续无需使用了需要系统恢复正常，执行以下代码：
```
cp /var/packages/SurveillanceStation/INFO /var/packages/SurveillanceStation/INFO.bak
sed -i 's/version="9.2.0-11289"/version="99.2.0-11289"/g' /var/packages/SurveillanceStation/INFO 
```
---

#以下为各群晖版本安装包下载地址以及破解脚本

### x86_64版本
- [安装包](https://global.synologydownload.com/download/Package/spk/SurveillanceStation/9.2.0-11289/SurveillanceStation-x86_64-9.2.0-11289.spk)
- 破解脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/9.2.0_11289/SurveillanceStation-x86_64/install_license)
```

---
### x86_64-openvino版本
- [安装包](https://global.synologydownload.com/download/Package/spk/SurveillanceStation/9.2.0-11289/SurveillanceStation-x86_64-9.2.0-11289_openvino.spk)
- 破解脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/9.2.0_11289/SurveillanceStation-x86_64_openvino/install_license)
```

---
### x86_64-DVA_3221版本
- [安装包](https://global.synologydownload.com/download/Package/spk/SurveillanceStation/9.2.0-11289/SurveillanceStation-x86_64-9.2.0-11289_DVA_3221.spk)
- 破解脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/9.2.0_11289/SurveillanceStation-x86_64_dva_3321/install_license)
```
---
### armada375版本
- [安装包](https://global.synologydownload.com/download/Package/spk/SurveillanceStation/9.2.0-11289/SurveillanceStation-armada375-9.2.0-11289.spk)
- 破解脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/9.2.0_11289/SurveillanceStation-armada375/install_license)
```

---
### armada38x版本
- [安装包](https://global.synologydownload.com/download/Package/spk/SurveillanceStation/9.2.0-11289/SurveillanceStation-armada38x-9.2.0-11289.spk)
- 破解脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/9.2.0_11289/SurveillanceStation-armada38x/install_license)
```

---
### armv7版本
- [安装包](https://global.synologydownload.com/download/Package/spk/SurveillanceStation/9.2.0-11289/SurveillanceStation-armv7-9.2.0-11289.spk)
- 破解脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/9.2.0_11289/SurveillanceStation-armv7/install_license)
```

---
### armv8版本
- [安装包](https://global.synologydownload.com/download/Package/spk/SurveillanceStation/9.2.0-11289/SurveillanceStation-armv8-9.2.0-11289.spk)
- 破解脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/9.2.0_11289/SurveillanceStation-armv8/install_license)
```

---
### 恢复默认授权
- 恢复脚本:
```
bash <(curl -L https://gitee.com/christianswift/surveillance-station-9/raw/main/9.2.0_11289/license/remove_license)
```
---
### 破解60授权效果
![License](https://gitee.com/christianswift/surveillance-station-9/raw/main/img/crack_license.png)



