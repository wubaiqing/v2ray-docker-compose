# V2Ray Docker 使用说明

### 服务端
1. 使用 [GGUID](https://www.guidgen.com/) 生成一个 ID 标识，然后打开 `./v2ray/config.json` 文件，修改[第 9 行](https://github.com/wubaiqing/v2ray-docker-compose/blob/master/v2ray/config.json#L9)的 ID 标识；
2. 可以从 [免费域名](https://www.freenom.com/zh/freeandpaiddomains.html) 申请一个域名，然后通过 [acme.sh](https://github.com/Neilpang/acme.sh/wiki/%E8%AF%B4%E6%98%8E)，申请证书；
3. 域名和证书下载后后缀不变，重命名为 **v2ray** 然后拷贝到 `./nginx/certs` 目录下；
4. 改变 `./nginx/conf.d/v2ray.conf` [第 8 行](https://github.com/wubaiqing/v2ray-docker-compose/blob/master/nginx/conf.d/v2ray.conf#L8)域名地址；
5. 使用 `docker compose up -d` 启动服务；

### 客户端
1. 从 [神一样的工具们](https://www.v2ray.com/awesome/tools.html) 下载当前环境的客户端；
2. 按下图设置客户端即可：
![](./images/client.png)


### 资源
GGUID 生成器：https://www.guidgen.com/  
免费域名：https://www.freenom.com/zh/freeandpaiddomains.html  
acme.sh：https://github.com/Neilpang/acme.sh/wiki/%E8%AF%B4%E6%98%8E