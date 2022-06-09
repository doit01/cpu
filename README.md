# cpu

 top -Hp 38330
 
 printf "%x\n" [线程id]
 printf "0x%x\n"  38740
  
  
 查出线程的16进制 为9754
 
 jstack  38330  |grep -C10 9754

jstack 38330 |grep -C10 CLogOracleWriterThread
