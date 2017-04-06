建立Dancer APP的两种方法
1）
	运行 dancer -a  myapp；
	在lib/myapp.pm 中直接配置对应路由；

	package Myweb;                                                                                                                                                  
	use Dancer ':syntax';

	our $VERSION = '0.1';

	get '/' => sub {
   		 template 'index';
	};
	
	...
	
	true;

2）	直接起一个脚本 myapp.pl
	
	#!/usr/bin/perl

	use Dancer;

	get '/' => sub{
        	return "HELLO WORLD!\n";
	};
	...
	start;