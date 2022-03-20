# 嵌入式代码模块

## 功能分类

- 主逻辑
- NRF24L01无线通信
- 定时器
- 电机模块  谢轶
- 运动功能
  - 移动
  - 击球
  - 吸球
- 通信协议
- PWM
- PID
  - 编码器
  - PID控制算法
- MPU传感器
- 蓝牙模块（实际使用较小）



## 文件分类

- action.c：动作执行函数，包括运动、击球、吸球、红外
- comm.c：无线通信数据处理，主要是通信协议
- gpio.c：GPIO初始化
- Hm_bluetooth.c：蓝牙模块串口通信协议
- i2c.c：i2c通信（比较复杂）
- init.c：硬件初始化，flash功能后面需要添加
- main.c：主程序（伪），实际主循环在robot.c
- misc.c：子功能函数
- moto.c：电机驱动，编码器，MPU
- MPU6050_driver.c：MPU陀螺仪驱动
- nrf24l01
  - nrf24l01_drv.c：无线通信模块驱动
  - nrf24l01.c：无线通信
- packet.c：通信协议，涉及接包，解包，发包等
- param.c：存储器默认参数
- pid.c：PID算法
- robot.c：控制器主程序
- timer.c：定时器相关程序
- Usart_ble.c：蓝牙串口通信协议

