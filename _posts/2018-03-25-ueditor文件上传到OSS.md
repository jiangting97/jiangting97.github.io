---
layout:     post
title:      OSS文件上传(ueditor1.4.3 OSS2.3.0)
subtitle:
date:       2018-03-25
author:     jiangting
header-img:
catalog: true
tags:
    - JS PHP
---
# 使用Ueditor上传文件到OSS

> 版本
> ueditor-php 1.4.3
> OSS 2.3.0


ueditor上传功能，首先会调用ueditor下php目录下的controller.php
比如我们要上传图片触发的action为uploadImage，调用action->upload.php,在此文件下实例化的
$up = new Uploader($fieldName, $config, $base64);是调用的Upload.class.php文件里的upFile方法上传文件

