## Career Experience

After I finished my Bachelor of Mechanical Engineering, I took a half-year trip to Yunnan. My career started in 2016 and continued until I began to pursue my post-degree in 2023 in Canada. During those 7 years, I took various roles.

### Junior Linux Driver Engineer

My first position was as a junior software engineer in an ODM company. As a newbie, I have a single duty of maintaining the audio system initially. After that, I quickly gained the trust of my colleagues and expanded my scope of functions to include more module drivers. During those 2 years and 4 months, I learned the Linux driver framework well and started to become proficient in C.

#### Android Audio Systems

This job is based on the Qualcomm platform. My responsibilities include:

1. Config the device tree to enable the Audio System.
2. Code the simple device driver based on the Advanced Linux Sound Architecture framework, such as an audio amplifier and headphone insertion detection.
3. Maintained and debugged the Android Hardware Layer audio module and modified it to match the customer's requirements.
4. Measure audio performance in a noise-cancelling room, including external amplifiers, headphones and noise cancellation.
5. Based on the measure results, use the software provided by Qualcomm to adjust the effect.

Since the Qualcomm platform provides quite complete and highly available code, and the increasing integration of audio devices reduces the difficulty of effect debugging, I had a lot of time to study the Linux driver in depth. At the same time, the company's business grows and lacks human resources. I had a chance to face the more challenging tasks.

#### Android USB drivers

I additionally take the role of the USB driver engineer. I need to work with our memory controller engineer and hardware engineer to bootload our development board and ensure debug tools, such as android-debug-bridge, work. Also, I need to customize our USB driver to match our customers' requirements.

My junior position was to help me build a solid foundation in C and Linux drivers. But most of the time, my role was to understand an existing driver code provided by a chip design company, then debug and modify it. I began to look forward to building a driver code from scratch and gaining a deeper understanding of the chip design process.

### Linux USB Driver Engineer

 My second career was in a WIFI apartment of a fabless semiconductor company. I got to conceptualize complete driver code and play an essential role in our team. During those 1 year and 8 months, I strengthened my knowledge of the USB bus and expanded my experience in the firmware area.

#### USB Linux Driver of WIFI chip

That WIFI chip can work both in USB high-speed, known as USB2.0, and SuperSpeed USB, known as USB3.0. Since it was designed for mobile devices, its requirements are strict high performance and low consumption.

When I joined that company, they had already finished verifying hardware design, and it was about 8 months before the tap-out. Since the USB driver was still empty, my schedule was tight. 

I first coded a simple driver code to verify the firmware functions, and then I started to discuss with our Linux middleware colleagues for user APIs and given a mock driver that they could start their work.

After finishing that, I used Python and C to make a unit test based on that mock driver, and then I started to design the driver. I paid a lot of attention to the interrupt handle and data competition. After 2 times refactoring, I got a satisfactory result.

During this development process, I understood the importance of the test-driven development model and have been practicing it in subsequent development practices.

Subsequently, we adapted USB controllers from other manufacturers, assisted them in debugging their controller drivers, and optimized our driver's performance.

#### WIFI HIFI Handset Firmware

After we successfully launched our chip, the production manager designed some demos to show the use case.

The WIFI HIFI headset utilizes WIFI’s high throughput for effective HIFI audio data transfer for higher performance than Bluetooth protocol. 

As the USB driver and universal DMA owner, I coded the USB module using interrupt transfers for control commands and isochronous transfers for audio data. My work on the universal DMA module is PCM data movement to the I2S interface. This whole system works in FreeRTOS and was developed by C.

### Senior Firmware Engineer