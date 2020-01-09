# storage2
/etc/udev/rules.d/99-oracle-asmdevices.rules
 
KERNEL=="sdb1" OWNER=="oracle", GROUP=="asmadmin", MODE=="0660"
KERNEL=="sdc1" OWNER=="oracle", GROUP=="asmadmin", MODE=="0660"
KERNEL=="sdd1" OWNER=="oracle", GROUP=="asmadmin", MODE=="0660"
 
[root@ihopedbsrv yum.repos.d]# chown oracle:asmadmin /dev/sdb1
[root@ihopedbsrv yum.repos.d]# chown oracle:asmadmin /dev/sdc1
[root@ihopedbsrv yum.repos.d]# chown oracle:asmadmin /dev/sdd1
[root@ihopedbsrv yum.repos.d]# chmod 660 /dev/sdb1
[root@ihopedbsrv yum.repos.d]# chmod 660 /dev/sdc1
[root@ihopedbsrv yum.repos.d]# chmod 660 /dev/sdd1
