# 蓝天p775tm(1)g系列10.13.6黑苹果配置


让你的蓝天p775tm(1)g吃上黑苹果

<!--[English](README.md) | 中文-->

## 电脑配置

| 规格     | 详细信息                                     |
| -------- | ---------------------------------------- |
| 电脑型号 | 蓝天 p775tm(1)-g             |
| 处理器   | 英特尔 酷睿 i7-9700k 处理器(8系也ok,我从8700升级到9700k的)             |
| 内存     | 32gb 海力士 DDR4 3200MHz                 |
| 硬盘     | 海康威视 NVMe固态硬盘 C2000PRO 1TB                  |
| 显卡 | Nvdia gtx 1060 ocg                           |
| 显示器   | 17.3寸 144hz 1080p ips  |
| 声卡     | 瑞昱 ALC899                    |
| 网卡     | KILLER E2500                              |



## 哪些不能在Clover正常工作

- 冷启动启动HDMI接口
  - 启动后再插入hdmi正常
- 风扇传感器
  - 无法查看风扇转速
- 杀手 1550网卡
  - 购买dw1560替代
- 睡眠
  - 菜单睡眠正常,快捷键睡眠和自动睡眠直接关机,待解决
- 雷电
  - 没有设备测试,未驱动
- 读卡器
  - 没有设备测试,未驱动
- 其他都工作正常



## 安装

使用黑果小兵[10.13.6 17G65](https://blog.daliansky.net/macOS-High-Sierra-10.13.6-17G65-Release-Version-with-Clover-4596-original-mirror.html)的镜像替换我的efi进行安装.系统安装完成后安装[Nvdia显卡驱动](https://images.nvidia.com/mac/pkg/387/WebDriver-387.10.10.10.40.105.pkg).最后更新系统到10.13.6 final版本.安装完成后驱动会不工作,不要紧张,进入驱动设置点击更新会自动安装适合的版本.

## 常见问题解答

### 插入hdmi接口外置显示器开机启动黑屏怎么办?

换成mini dp接口即可.(hdmi可以在开机启动后插入)

### 需要驱动四条内存怎么办?

使用config_imac.plist文件启动即可

## 更新日志
2019.10.16

- 更换机型为MacBookPro13,3 
- 备份imac机型的config文件

2019.09.29

- 更新readme
- 更新dw1560驱动

