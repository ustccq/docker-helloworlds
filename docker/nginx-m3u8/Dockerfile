# 使用官方的 Nginx 镜像作为基础镜像
FROM nginx:latest

# 在容器中创建一个目录用于存放你的文件
RUN mkdir /usr/share/nginx/stream

# 将本地的 stream 目录下的文件拷贝到容器的目标目录
COPY ./stream /usr/share/nginx/stream

# 在原始 nginx.conf 文件的 server 块中添加你的 location 指令
COPY Default.conf /etc/nginx/conf.d/default.conf

# 暴露 Nginx 监听的端口
EXPOSE 80

