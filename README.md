# playPony

## QQ空间宠物自动化脚本

### 版本说明

v1.php：每次运行，自动偷糖果、喂食（包括好友）、捡大便（包括好友）

v2.php：在v1的基础上修正+只喂食暮光闪闪

### 安装

新建`config.php`文件，填入：

```
define('QQNUM', 'QQ号');
define('SKEY', 'QQ空间skey');
define('PSKEY', 'QQ空间p_skey');
define('FOOD_LIMIT',0);//每次运行喂食次数限制，0为不喂食
```

设置文件权限：

	chmod -R +x /path/to/playPony/

将`v1.php`或`v2.php`加入cron，每五分钟运行一次，输出日志到log.txt：

	*/5 * * * * php /path/to/playPony/v2.php >> /path/to/playPony/log.txt 2>&1
	

## LICENSE

GPLv3