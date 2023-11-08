<h2 align="center">
    Windows配置PHP多版本服务
</h2>

## 介绍

windows下PHP多版本配置模板

## 安装

### `clone`仓库代码:

```bash
git clone https://github.com/chendujin/win-multi-php.git
```

### 配置环境变量
在windows设置 - 高级系统设置 - 环境变量 的Path中添加：
```bash
D:\Code\win-multi-php\server
D:\Code\win-multi-php\php

# 这里配置默认的PHP版本，即可直接运行：php -v
D:\Code\win-multi-php\php\php-8.0.29
```
> 注：上面的路径 `D:\Code\win-multi-php\` 替换为自己的路径即可

## 安装Composer

自行谷歌/百度安装即可,这里不再进行赘述。

## 使用示例
```bash
# 查看PHP版本信息
php -v
php56 -v
php71 -v
php72 -v
php73 -v
php74 -v
php80 -v
php81 -v
php82 -v

# 查看是否安装某个配置
php -m|grep swoole

# 查看某项具体配置信息
php -i|grep disable_functions

# 查看某个扩展具体信息
php --ri swoole 
```