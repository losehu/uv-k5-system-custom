# uv-k5-system-custom
* This repository is for simulating the loading of firmware larger than 64KB on UVK5, up to 512MB.
* Developers only need to modify the ld file.

# uv-k5-system-custom
* 这个仓库用于实现在UVK5上加载超过64KB固件的模拟器，最大512MB
* 开发者只需要修改ld文件
  
# Principle
* The firmware is stored in blocks in memory.
* Simulates the state of each register, parses jump instructions, and analyzes the stack state.
* Redirects jump instructions and the stack.
* Saves the state to the system's stack register on every jump.
* Redirects to the firmware's vector table in the system's interrupt function to jump to the firmware's interrupt functions.

# 原理
* 将固件分块存放在内存中
* 对每个寄存器状态模拟，解析跳转指令，解析堆栈状态
* 将跳转指令、堆栈重定向
* 在每次跳转都将状态保存到系统的堆栈寄存器
* 在系统的中断函数内重定向到固件的向量表，从而跳转到固件的中断函数

# Challenges
* This mechanism is difficult to guarantee communication timing.

# 困难
* 这种机制难以保证通讯的时序

# Contact Me
* If you have good suggestions or ideas, feel free to reach out and discuss.
* I welcome any form of technical exchange.

# 联系我
* 如果你有好的建议和想法，可以与我交流，
* 我十分欢迎任何形式的技术交流

* ![t_me-Fizver](https://github.com/user-attachments/assets/fa906e15-c40c-4a97-a7d0-af5d0d7e89f8)

