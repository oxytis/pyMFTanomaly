$MFT timestomping and tunneling detection
================

mft anomaly - forensic timestamp tampering and file tunneling detection

<b>prerequisites</b> <br>

tzworks.net -> ntfswalk64 

<b>execution</b>
1) ntfswalk64 -mftfile $MFT > mftfile<br>
2) python mft.py mftfile stomp ""<br>
     or<br>
   python mft.py mftfile stomp "" | "Users\user" <-- only this directory<br>
     or<br>
   python mft.py mftfile tunnel "filename" <-- only check for this filename<br>

<b>output</b>

ANOMALY---

     \[root]\<path corrupted>\p\pfBL.dll
     $STD_INFO:  01/03/2018   13:33:44.000 
     $FILE_NAME: 11/19/2019   17:09:09.403

SUMMARY...


     ('2023-03-20', 1)
     ('2023-04-11', 1)
     ('2024-02-20', 1)
     ('2023-02-21', 5)
     ('2022-12-19', 5)
     ('2022-12-15', 6)
     ('2023-08-30', 121)
