# cpu

cpu load 过高
用top 查看到running task 20多。 过一会降到了2个
用 ps aux | less 查看哪些是运行的 r表示运行的。
 

 top -Hp 38330
 
 printf "%x\n" [线程id]
 printf "0x%x\n"  38740
  
  
 查出线程的16进制 为9754
 
 jstack  38330  |grep -C10 9754

jstack 38330 |grep -C10 CLogOracleWriterThread
