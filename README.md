小程序AppID：wxc1ce4c6809c6fafe


163网易邮箱
账号：zyq3252196042@163.com
密码：3252196042



天天生鲜发送邮件

# 发送邮件配置
EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
# smpt 服务地址
EMAIL_HOST = 'smtp.163.com'
EMAIL_PORT = 25
# 发送邮件的邮箱
EMAIL_HOST_USER = 'zyq3252196042@163.com'
# 在邮箱中设置的客户端授权密码
EMAIL_HOST_PASSWORD = 'zyq3252196042'
# 收件人看到的发件人
EMAIL_FROM = '天天生鲜<zyq3252196042@163.com>'


# 发送邮件配置
EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
# smpt服务地址
EMAIL_HOST = 'smtp.qq.com'
EMAIL_PORT = 25   # 端口默认都是25不需要修改
# 发送邮件的邮箱，需要配置开通SMTP
EMAIL_HOST_USER = '3252196042@qq.com'
# 在邮箱中设置的客户端授权密码
EMAIL_HOST_PASSWORD = 'whqwleishwtwcjji'
# 收件人看到的发件人
EMAIL_FROM = '带签名的<3252196042@qq.com>'


pip insall eventlet
启动celery异步： celery -A celery_tasks.tasks worker -l info -P eventlet（cmd中进入项目所在目录）

# Django的redis缓存配置
CACHES = {
    'default':{
        'BACKEND': 'django_redis.cache.RedisCache',
        'LOCATION': 'redis://127.0.0.1:6379/9',
        'OPTIONS': {
            'CLIENT_CLASS': "django_redis.client.DefaultClient",
        }
    }
}

# 配置session存储
SESSION_ENGINE = 'django.contrib.sessions.backends.cache'
SESSION_CACHE_ALIAS = 'default'
192.168.145.130

FastDFS上传文件和nginx启动：
启动tracker 和 storage
sudo service fdfs_trackerd start
sudo service fdfs_storaged start
fdfs_upload_file /etc/fdfs/client.conf 要上传的图片文件 
启动nginx
sudo /usr/local/nginx/sbin/nginx（或者: 1. cd/usr/local/nginx/sbin 2. sudo ./nginx）

关闭nginx：sudo /usr/local/nginx/sbin/nginx -s stop

关闭防火墙：
systemctl stop firewalld


BYY:
sudo apt-get update
sudo apt-get install git
sudo apt-get install liberror-perl
sudo apt install build-essential


