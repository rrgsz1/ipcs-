# ipcs-

ipcs用法：

是linux/uinx上提供关于一些进程间通信方式的信息，包括共享内存，消息队列，信号
ipcs用法 
ipcs -a  是默认的输出信息 打印出当前系统中所有的进程间通信方式的信息
ipcs -m  打印出使用共享内存进行进程间通信的信息
ipcs -q   打印出使用消息队列进行进程间通信的信息
ipcs -s  打印出使用信号进行进程间通信的信息
输出格式的控制
ipcs -t   输出信息的详细变化时间
ipcs -p  输出ipc方式的进程ID
ipcs -c  输出ipc方式的创建者/拥有者
ipcs -c  输出ipc各种方式的在该系统下的限制条件信息
ipcs -u  输出当前系统下ipc各种方式的状态信息(共享内存，消息队列，信号)

ipcrm 命令 ：

移除一个消息对象。或者共享内存段，或者一个信号集，同时会将与ipc对象相关链的数据也一起移除。当然，只有超级管理员，或者ipc对象的创建者才有这项权利啦
ipcrm用法 
ipcrm -M shmkey  移除用shmkey创建的共享内存段
ipcrm -m shmid    移除用shmid标识的共享内存段
ipcrm -Q msgkey  移除用msqkey创建的消息队列
ipcrm -q msqid  移除用msqid标识的消息队列
ipcrm -S semkey  移除用semkey创建的信号
ipcrm -s semid  移除用semid标识的信号
