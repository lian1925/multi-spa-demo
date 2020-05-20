## docker 验证
1、安装nginx 镜像
```
docker pull nginx:1.17.10
```

2、运行容器

```
docker run --name nginx-demo -p 80:80 -v /Users/huahua/Documents/lian/code/multi-spa-demo/project-a/dist/:/usr/share/nginx/html/a:ro -v /Users/huahua/Documents/lian/code/multi-spa-demo/project-b/dist/:/usr/share/nginx/html/b:ro -v /Users/huahua/Documents/lian/code/multi-spa-demo/nginx.conf:/etc/nginx/nginx.conf:ro -d nginx:1.17.10
```
