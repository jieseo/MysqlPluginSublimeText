# MysqlPluginSublimeText
mysql操作命令快捷方式

## 一、插件安装
将mysqlPlugin目录复制到Sublime Text 3的安装目录
```html
Sublime Text 3\Data\Packages\User 
```
此目录下即可使用


## 二、如何使用
在文件中键入：createtable 后，按TAB键生成代码：
```html
CREATE TABLE `tb_user` (
   `id` int(10) unsigned NOT NULL AUTO_INCREMENT COMMENT '用户ID',
   `username` varchar(40) DEFAULT '' COMMENT '用户登录名',
   `password` char(32) DEFAULT NULL COMMENT '密码',
   `nickname` varchar(50) NOT NULL COMMENT '别名',  
   `usertype` tinyint(1) NOT NULL DEFAULT '0' COMMENT '0:普通',
   `wealth` bigint(20) unsigned NOT NULL DEFAULT '0' COMMENT '财富等级',
   `signature` text COMMENT '用户签名',   
   PRIMARY KEY (`id`),
   KEY `username` (`username`)
 ) ENGINE=InnoDB DEFAULT CHARSET=utf8
 ```

 大家有什么命令一起补充。