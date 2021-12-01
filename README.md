# pnet
a simple shell program for monitor a custom process's network traffic on every network device

**usage**
`usage: pnet -p <pid> [-t <seconds>] [-h]`

**exmaple**
monitor process pid 1 network traffic every 5 seconds
```
root@pc /]# pnet -p 1 -t 5
------------------------------pid:1,time:18:34:09-------------------------------
|interface      | |recv(KB)  |tran(KB)  | |recv(MB)  |tran(MB)  | |recv(GB)  |tran(GB)
|virbr0-nic     | |0         |0         | |0         |0         | |0         |0
|virbr0         | |2964923   |4839500   | |2895      |4726      | |2         |4
|enp2s0         | |5486052   |79        | |5357      |0         | |5         |0
|enp3s0         | |1829876883|6899078801| |1786989   |6737381   | |1745      |6579
|lo             | |930632828 |930632828 | |908821    |908821    | |887       |887
|docker0        | |2577      |54699     | |2         |53        | |0         |0
------------------------------pid:1,time:18:34:14-------------------------------
|interface      | |recv(KB)  |tran(KB)  | |recv(MB)  |tran(MB)  | |recv(GB)  |tran(GB)
|virbr0-nic     | |0         |0         | |0         |0         | |0         |0
|virbr0         | |2964923   |4839500   | |2895      |4726      | |2         |4
|enp2s0         | |5486052   |79        | |5357      |0         | |5         |0
|enp3s0         | |1829877110|6899078926| |1786989   |6737381   | |1745      |6579
|lo             | |930634783 |930634783 | |908823    |908823    | |887       |887
|docker0        | |2577      |54699     | |2         |53        | |0         |0
```
