# cpu
top 
 top -Hp 38330
 查出线程的16进制 为9754
 jstack  38330  |grep -C100 9754
