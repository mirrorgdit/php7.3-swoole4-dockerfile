## php7.3-swoole4.4.5-dockerfile
php7.3-swoole4.4.5-dockerfile  可构建后用于基于的swoole相关的项目框架，如hyperf,easyswoole,mixphp等等

## 简介
Docker File ，可构建后用于基于的swoole相关的项目框架，如hyperf,easyswoole,mixphp等等。


## 1.创建镜像
```
docker build -t yourImageName .# 使用此目录的 Dockerfile 创建镜像(当前目录 记得.号)

例如：docker build -t hyperf/hyperf .   
```

## 2.容器外代码挂载
可自行将项目代码挂载到docker内,例如swoole框架hyperf的项目：
```
docker run -p 9501:9501 -v /home/wwwroot/hyperf-skeleton:/home --name hyperf hyperf/hyperf:latest php /home/bin/hyperf.php start
```

```
在/home/wwwroot/hyperf-skeleton下进行代码开发，代码修改后可重启容器刷新代码 docker restart hyperf
```

## 问题反馈

在使用中有任何问题，欢迎反馈给我，可以用以下联系方式跟我交流

Email：[mirrorgdit@163.com]



