# 使用官方的 Nginx Alpine 镜像作为基础镜像
FROM nginx:1.29.0-alpine

# 更新包索引并安装 bash
RUN apk update && apk add --no-cache bash

# 设置工作目录（可选）
WORKDIR /usr/share/nginx/html

# 拷贝本地的nginx配置文件（可选）
# COPY ./nginx-conf /etc/nginx/conf.d

# 暴露80端口
EXPOSE 80

# 启动nginx
CMD ["nginx", "-g", "daemon off;"]
