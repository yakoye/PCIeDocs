PCIe的吞吐量是什么


PCIe的吞吐量是指PCIe链路的可用带宽，即每秒钟能够传输的有效数据量。PCIe的吞吐量与传输速率、编码方案、链路宽度等因素有关。¹

PCIe的传输速率是指每一条Lane上每秒钟能够传输的位数，用GT/s（千兆传输/秒）表示。PCIe的传输速率与不同的版本有关，例如PCIe 1.0为2.5 GT/s，PCIe 2.0为5 GT/s，PCIe 3.0为8 GT/s，PCIe 4.0为16 GT/s，PCIe 5.0为32 GT/s或25 GT/s。¹

PCIe的编码方案是指物理层协议中使用的数据编码方式，用于提高信号质量和可靠性。不同的编码方案会导致不同的开销位，从而影响吞吐量。例如PCIe 1.x和PCIe 2.x使用8b/10b编码方案，即每传输8个bit，需要发送10个bit；而PCIe 3.x和PCIe 4.x使用128b/130b编码方案，即每传输128个bit，需要发送130个bit。¹

PCIe的链路宽度是指一条PCIe链路由几条Lane组成，用x1、x2、x4、x8、x16等表示。不同的链路宽度会影响吞吐量的倍数。例如x1表示一条Lane，x4表示四条Lane，x16表示十六条Lane。¹
根据以上因素，可以计算出PCIe的吞吐量公式为：

吞吐量 = 传输速率 x 编码方案 x 链路宽度 x 2

其中2表示全双工通信。


举例说明：
PCIe 2.0 x8的吞吐量为：5 GT/s x (8/10) x 8 x 2 = 64 Gbps = 8 GB/s

PCIe 3.0 x16的吞吐量为：8 GT/s x (128/130) x 16 x 2 = 126.031 Gbps = 15.754 GB/s

PCIe 4.0 x4的吞吐量为：16 GT/s x (128/130) x 4 x 2 = 31.508 Gbps = 3.939 GB/s



(1) PCIe传输速率和可用带宽（吞吐量）计算 - CSDN博客. https://blog.csdn.net/s_sunnyy/article/details/79027379.

(2) 【精讲】PCIe基础篇——PCIe传输速率计算 - CSDN博客. https://blog.csdn.net/u013253075/article/details/108926633.

(3) PCIe传输速率、吞吐量、PCLK计算方式 - CSDN博客. https://blog.csdn.net/sinat_43629962/article/details/123729771.