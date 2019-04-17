# 问题及解决汇总

Problem：在gpio_led_output的demo中，在程序中修改没有实现LED颜色变化的功能    
Solution：原因在于没有修改demo的配置文件。除了主程序中要修改并添加相应的LED灯的GPIO端口组和相应引脚，还必须要修改LED灯引脚配置文件，不然默认的初始化函数不会初始化引脚。  

在新建项目时，若要使用UART，则需要使用Default board files
