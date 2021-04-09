
FROM php:5.4.45

#COPY ./resources/sources.list /etc/apt/

#WORKDIR /tmp

# 安装 redis 扩展
#ADD ./resources/redis-5.1.1.tgz .
#RUN mkdir -p /usr/src/php/ext \
#    && mv /tmp/redis-5.1.1 /usr/src/php/ext/redis \
#    && docker-php-ext-install redis
#
# 以下注释按需打开（某些项目需要 npm 啥的）
# 安装 python3
#ADD ./resources/Python-3.8.0.tgz .
#RUN cd /tmp/Python-3.8.0 && ./configure && make && make install && rm -rf /tmp/Python-3.8.0 Python-3.8.0.tgz

# 安装 nodejs
#ADD ./resources/node-v12.13.0-linux-x64.tar.xz .
#RUN ln -s /tmp/node-v12.13.0-linux-x64/bin/node /usr/bin/node \
#    && ln -s /tmp/node-v12.13.0-linux-x64/bin/npm /usr/bin/npm

# 安装 swoole
#ADD ./resources/swoole-src-4.4.12.zip .
#RUN cd /tmp && unzip swoole-src-4.4.12.zip \
#    && cd swoole-src-4.4.12 && phpize && ./configure \
#    && make && make install && rm -rf /tmp/swoole*

# 安装 mcrypt
#ADD ./resources/mcrypt-1.0.3.tgz .
#RUN cd /tmp/mcrypt-1.0.3 && phpize && ./configure && make && make install && rm -rf /tmp/mcrypt-1.0.3
#RUN cd /usr/src/php/ext/mcrypt && phpize && ./configure && make && make install

# 安装 mongodb
#ADD ./resources/mongodb-1.6.0.tgz .
#RUN cd /tmp/mongodb-1.6.0 && phpize && ./configure && make && make install && rm -rf /tmp/mongodb-1.6.0

# 安装 swoole_loader73.so
#COPY ./resources/swoole_loader73.so /usr/local/lib/php/extensions/no-debug-non-zts-20180731/
CMD php-fpm
