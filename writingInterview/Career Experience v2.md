## Career Experience

During my 7 years of experience, I developed various systems. Based on the Canonical written interview question, I listed 3 projects in order by date. 

I described the details of the project at the start of each section and the list of my responsibilities after that.

### Android Audio Systems

My software engineering career started in embedded Linux. I was an Android Audio System engineer in my first company. My responsibilities were configuring, adjusting and debugging audio systems based on the Qualcomm platform. Since Qualcomm provided detailed documentation and completed codes, its learning curve is smooth, and that position allowed me to learn a wide range of technologies:

1. Linux Device Tree: I need to enable and select the correct audio system modules
2. Advanced Linux Sound Architecture: I need to debug and develop the audio device based on it.
3. I2S, I2C and SPI: Those peripheral buses are used in most audio devices
4. The audio component of the Android Hardware Abstract Layer (HAL): It is a middleware layer between the Linux driver and user space, written in C++. I need to debug it to support our application developer.
5. Basic audio noise cancellation principles: I need to measure audio performance in a noise-cancelling room, including external amplifiers, headphones and noise cancellation and use the software provided by Qualcomm to adjust the effect.

### The Solid-state drive Controller Firmware

This project came from my third company, an enterprise store solution with hardware compress. This makes it quite complex and has a low tolerance for errors. Its firmware code is based on the ARM A55 without an operating system to exclude the additional overhead caused by thread switching. We developed it based on C++.

1. I developed algorithms for garbage collection and were-levelling
2. I was involved in the hardware design verification and finished the verification for the Coherence Hub Interface (CHI) and the Direct Memory Access (DMA) module.

#### The Unit Test Code System

I want to highlight the unit test code system of this SSD controller firmware. Because of the low tolerance for errors, we decided to develop a simulator for our hardware. Based on that simulator, we can make mock data and build a special situation to test our firmware. Furthermore, in order to test our simulator, we developed a set of unit tests, which we also used in the hardware design verification.

1. I developed the simulator module for the CHI module and the DMA module.
2. I developed the unit test of the CHI and DMA modules, and as a result, I successfully located a coherence problem between DMA and Arm Advanced High-performance Bus (AHB) in our FPGA prototype.

### AI Accesstor

The production of my last company is an enterprise AI Accesstor card for Linux servers. As a startup company, when I joined it, we faced an extreme human source shortage. Therefore, I took on a lot of tasks:

1. I designed and coded the Linux PCIe driver.
2. I designed and implemented the firmware of the PCIe controller.
3. I address and improve the software performance, including the PCIe driver, PCIe firmware and AI compiler.
4. I provided and implemented the Python APIs for the QA team to test the firmware and driver.
5. I provided and implemented the APIs for the K8S team for the virtualization function.

#### Address and improve the software performance

I did a lot of work related to software performance for the last company. I would take different steps in both cases: Based on Linux or based on firmware.

Based on Linux, Linux offers complete toolchains for us. I would first use the command `perf` to record the stack trace information, then use the Flame Graph to analyze it.

Based on firmware, it would be more complex. If we have a central process scheduler, I will use the macro to add some debug code to determine if some process executing time is unexpected. If we didn't have a central process scheduler, we need to analyze the code and try to address the hot code. Adding some time stamp logs will be helpful.

#### Package the driver and middleware layer for the QA team and K8S team

We didn't share the source code with the QA team and K8S team. Instead of that, we package our driver and middleware layer into `.deb` file and `.rpm` file. I was involved in configuring GitLab's CI pipeline for that.

### Topics outside the project

#### How do you think about and ensure quality in your software products?

There are two aspects to the "quality of software products". First, code robustness. My ultimate answer is "completely, automatically unit test." Second, code readability and maintainability. It's harder than the previous one. I believe the deliberate architecture, code refactoring, proficient programming skills and complete documents will help us achieve that goal.

#### How do you prefer to drive documentation for your products?

I have gone through multiple teams that had different documentation processes. But no matter what kind of documentation process they use, they all face the problem of documentation decay.

I personally have a good habit of recording the results of my work every day at the end of the day. This process helps me in many ways, including self-reflection, time management, and document writing. It will help me to figure out which document I need to update and provide detailed materials.

It also helped me complete this detailed written interview.

#### Programming language

My C language programming skills have been practiced in many projects, and I think I am a proficient C language user.
